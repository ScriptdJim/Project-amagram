# CD12352 - Infrastructure as Code Project Solution
# [ Hello reader, is Abasiama .J. ]

## Spin up instructions
First off, you want to cd(change directory) into the correct directory.
> cd Project-solution

Run these to check if the necessary installations have been installed. 
// View all existing profile names.
> aws configure list-profiles
if there are any available profiles, choose one and begin step 2, If not begin step 1. 

Step 1. Configure AWS (preferably adding a new profile for udacity) 
> aws configure --profile amagram

Step 2. Create network infrastructure
> ./create_net.sh --profile amagram

Step 3. Create server infrastructure
> ./create_amagram.sh --profile amagram
// Once completed running, You should then see web page:  
> "It works! Udagram, Udacity!"

## Tear down instructions
TODO
To delete the application infrastructure:
> ./delete_udagram.sh --profile amagram

To delete the network infrastructure:
> ./delete_net.sh --profile amagram

## Other considerations
TODO (optional)
I have some files in the Project solution directory:

# net.yml:
// The network infrastructure also used by the create_net.sh and update_net.sh scripts.
# net_params.json: 
// The parameters for the network infrastructure.
# amagram.yml 
// The application resources.
# amagram-params.json
// The parameters for the application infrastructure.
# amagram-bonus.yml
// This is the solution to the bonus section of the assignment. 
# update-amagram.yml
// This is to update the infrastructure with an additional section to the basic already running stack. 


# Project-amagram
