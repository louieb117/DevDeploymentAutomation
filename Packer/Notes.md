# Packer Notes

## Resources
Link: https://xcp-ng.org/blog/2024/02/22/using-packer-with-xcp-ng/

This implementation was based off the guide provided above. Worked pretty well. preseed file needed some modification. The late_command strings did not work. Ended up manually added the line to the config file and manually installed guest tools.