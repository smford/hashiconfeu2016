#
# DO NOT DELETE THESE LINES!
#
# Your DNSimple email is:
#
#     sethvargo+terraform@gmail.com
#
# Your DNSimple token is:
#
#     1Gam3SE2eIwZYtq70H5V5iAXiE9sGPmf
#
# Your Identity is:
#
#     hashiconf-34173cb38f07f89ddbebc2ac9128303f
#
provider "dnsimple" {
    token = "${var.dnsimple_token}"
    email = "${var.dnsimple_email}"
}

resource "dnsimple_record" "web" {
	domain = "terraform.rocks"
	type = "A"
	name = "stephenf"
	value = "${aws_instance.web.0.public_ip}"

}
