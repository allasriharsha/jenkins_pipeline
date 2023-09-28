

pipeline {
    agent any
environment {
        SSH_KEY = credentials('-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEApYgBQtZvv5WJcFluTc6ZJZaUtZ5b0wb3S9CiaohfXOtxdf+0
xm1wNG3lNbXaMIzm2eMiFu79c1XxHnV+Aehs9RfaF4AdLTB0KW5M1GNmENUaXOIW
9pjt28l85+BtPY7OkgzPMSDCVZ7Uxo86NTPJXU+nmw/cGUd9XmWJ9RM0nePZczym
ImJPKwESKYNouQFo1Sye/9pw/nNuOA89EAUhUPyuyl03FibIqrkfnY7aWPa5VhZt
G2kB5b4v+68KQNtGM/S2bzEgpBy+A0e3pV9JC2NaIy+kfmC8LKUaiVSeg1wyfk18
aSSM8dvuAmI1SNQoQPl1gUHyw5IccrBZiAdD/wIDAQABAoIBAADQNEFh0Fa+o1g7
+EDFnRcEMGLcDlNxG1HyCno/hUhtl7cetIKtEvoO+CtVY2cNqiyz4vz925zvdSnT
JfVYcQCbR2UKKhqIvGlfs1zvyBaZFXITYk1/3ttPmB+DiMXep8Er8vCo2ouVJjJ7
jaupP3oH5Cjs4QX2xfTqxsy/dWi5Ldgz86lIsLonYayd9DLm4IVtEA3wsoJ1Fpd7
rJ8T5hdd5FooB3lg60g4M9X7KD0tjWVmsPyxiWaNjc/oLrGJZAjQ70kIH9skRER3
0QxyYEJ8O1VlhdQNZUEZ9b6fzfrM1Loy671bKz5vk85s03Y2MRQOT+8JPQ0bppWp
cG2lwuECgYEA1LNqb2O5+0hqHKZq26uZVZ9oNms/osDzll6eniKqJC93SIatSVNN
XlaWE58ZCxcjlYtNvFWybaUB0H1plKih/lBTFcfnMnNI4NqC0plTbBJ0GJMzRKT7
ducNHC7/vcArMwnbCCZfVyZ4D8Z/ZYKGwHs551bcJzeMXEyObGP1vicCgYEAxzpq
97/30ms/pGuKYwfH7/zbFRmSf2jAM55laERlMJjJ/t81yakYfhgf0psWOx1rVFN1
stn3smSMYYMLvV7qHmIQ2ewheRwPKnz5wEQn7DAyLsb1ClLbfIdpNYpkTGfp0h1F
+zIluhV4WKqwBQMADog4aIWwdWh7qNgzWGazSmkCgYAAvJpaxmqnfym27bCjECYY
0NOIlLiEtMxjMfK0s4QJWgy8uJKzFVHISN5+NOfeTPc3lmLvixByJscp1LVf6XGe
MuMGyUl4uEOBW+BmIFfUoP+78g6UZ0njsIswFM2X96lupNMYZSGhaKWz0EkyrdAP
rJ2XuopKrHuU+kLoBzSbswKBgAHAQbBrv4HZ73VCfLTiHJ+/WS2WS/NSuF27xqhj
8X+72Aqla5OaKNzy2VTAiDF80LStBxvLTqICwDkbLb88VlJuCjfgG2s1E+0LrCZE
cxVgVxCSLxUoJUWy6vnNfZQuVZ/DIhpTFoHMLoKY/XMN07JNADHq+uINSQjy3YCp
ZmoBAoGAAt2sWWT0TKWmPHzLoEv1sunA9mzvf6Pks6Y+n2VFmPuIJvOg6ijT97b+
cuYHRRvOW6UpwsIG+C2lHzsVUEG23AwVkwP/rAesLXldolkh1FdpotJhe2/g0JfK
DQ0q4QpVj3/kmjGJJVeOagDIcjKpQgtkmANkk/397OBCSONbT8s=
-----END RSA PRIVATE KEY-----')
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo Building...'
                sh 'echo "Using API key: $SSH_KEY"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo Testing...'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo Deploying...'
            }
        }
    }
}
