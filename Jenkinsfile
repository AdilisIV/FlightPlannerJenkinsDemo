node {
    checkout scm
    def the_one_to_run
    
    if (env.BRANCH_NAME == "master"){
        the_one_to_run = load 'master.groovy'
    } else {
        the_one_to_run = load 'not-master.groovy'
    }
    
    the_one_to_run.run_build()
}