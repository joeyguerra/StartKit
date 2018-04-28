node {
	stage 'Checkout and Setup'
		checkout scm
	stage 'Lint'
		sh 'bundle exec fastlane custom_lane'
	stage 'Test'
		sh 'bundle exec fastlane test'
	stage 'Build'
		def build_number = env.BUILD_NUMBER
		sh "bundle exec fastlane build build_number:${build_number}"
	stage 'Deploy'
		archive 'reports/, dist/'
		sh 'bundle exec fastlane deploy'
}
