node{
    stage('Checkout SCM'){
    sh "git clone https://github.com/johnpapa/angular-tour-of-heroes.git David"
    sh "cd David"  
    }
    stage('Install node module') {
    sh "npm i"
    sh "npm cache clean --force"
    sh "npm install @angular-devkit/build-angular@0.13.0"
    }
    stage('Build') {
    sh "npm run build --prod"
    }

    stage('Deploy') {
    sh "ng serve"
    }
}
