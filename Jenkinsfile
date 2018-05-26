pipeline{
agent any
stages{
stage ('Test'){
steps {
echo "running the test stage"
  sh 'ant -f test.xml-v'
  junit 'reports/result.xml'
  echo "exiting the test stage"
}
}
stage ('build') {
steps{
echo "This is my build stage"
  sh 'ant -f build.xml -v'
  echo "build completed"
}
}
}
}
