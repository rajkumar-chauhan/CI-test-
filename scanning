provider "aws" {
  region = "us-east-2"
}

provider "aws" {
  region     = "us-west-2"
}

resource "aws_instance" "web" {
  ami           = data.aws_ami.ubuntu.id
  instance_type = "t2.micro"

  tags = {
    Name = "HelloWorld"
  }
}
