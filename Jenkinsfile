node {
	stage 'Checkout and Setup'
		checkout scm
	stage 'Lint'
		sh 'bundle exec fastlane ios lint'
	stage 'Dependency Management'
		sh 'bundle exec fastlane carthage_update'
	stage 'Test'
		sh 'bundle exec fastlane ios run_test'
	// stage 'Build'
	// 	def build_number = env.BUILD_NUMBER
	// 	sh "bundle exec fastlane build build_number:${build_number}"
	// stage 'Deploy'
	// 	archive 'reports/, dist/'
	// 	sh 'bundle exec fastlane deploy'
}
