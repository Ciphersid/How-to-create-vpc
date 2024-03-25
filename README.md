# How-to-create-vpc

what vpc in aws !
It is a region level conatiner which is used to divide big network into segment
it uses more subnet concept because it uses cidr vaalue while creating subnet
cidr full form classeless inter domain range
cidr example: - 192.168.0.0./24
	if we have an ip address like 192.168.0.0 - 192.168.255.255
it means from 255network could be build and 255 each network will get 255 host and i think its enough for any organization

Network like , let assume that we have open on college and there are 4 department and we have to provide interconnectivity with their
respective department then how will come into subnetting let see

college have we will provide one network to each deaprtment using under created vpc and
vpc ip address is 192.168.0.0/16 it means from 255network could be build and 255 each network will get 255 host  :-
but now we will assuming 4 department only thats y we will create only 4 network as follows

i will use this range in this subnet 192.168.1.0/24  what this ip explaining that i am in network 1 and in my network i can persue 255 host only simple.
IT department
192.168.1.0/24
CS department
192.168.2.0/24
Bms Department
192.168.3.0/24
bcom Department
192.168.4.0/24
now subnet concept over

now we will see internet gateway
u will see inter gateway i have created one intergate way using my
attach it to created vpc already
now to edit subnet route table which won't be able to surf with internet remove anywhere
after it go and create one more route table in which private subnet to be add and
after it create one private instance and first select vpc after it select subnet in subnet you should slelect
your desire subnet either private or public or else and then disable ssh
for testing you should have to allow icmp ipv4 protocol in your private instance beacause ping uses icmp protocol for pinging.

