pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Mengambil kode dari repository GitHub...'
                // Jenkins otomatis melakukan checkout dari SCM
            }
        }
        
        stage('Build / Compile') {
            steps {
                echo 'Menjalankan proses build...'
                // Tambahkan perintah build Anda di sini, contoh: sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Menjalankan unit testing...'
                // Tambahkan perintah testing di sini, contoh: sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Melakukan deployment aplikasi...'
                // Tambahkan perintah deploy di sini
            }
        }
    }

    post {
        always {
            echo 'Pipeline selesai dijalankan.'
        }
        success {
            echo 'Build BERHASIL! 🎉'
        }
        failure {
            echo 'Build GAGAL! ❌ Silakan periksa log.'
        }
    }
}
