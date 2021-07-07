pipeline {
    agent any
    stages {
        stage("Newman Test") {
    	    steps {
                echo "Starting Newman Test"
                bat "C:/Users/maria/AppData/Roaming/npm/newman run --disable-unicode https://www.getpostman.com/collections/927fcdc629c39e9b4fd6 --reporters html --reporter-html-export D:/MarianOptimal/PostmanCollection/newman/report-mule.html"
            }
        }
        stage("JMeter Loading Test") {
            steps {
                echo "Starting the JMeter Loading Test"
                bat "C:/Users/maria/Downloads/apache-jmeter-5.4.1/apache-jmeter-5.4.1/bin/jmeter -jjmeter.save.saveservice.output_format.xml -n -t D:/MarianOptimal/JMeter/mule-products.jmx -l D:/report-mule.jtl"
            }
        }    
    }
}
