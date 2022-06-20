# creating-modifying-deleting-config

Implementation Config Lambda = modify_config
•	Enable config in the account when it's disabled. If config recorder is not on, turn it on for config to get configuration changes.
•	If Config is already configured, get the log bucket where it's logged, check against existing GD set bucket, set the log bucket to GD central logging bucket.
•	No changes are needed for Config turned on and that have a storage location set to GD Central logging bucket.

![Copy of Copy of AWS Solution Architect-Associate (2)](https://user-images.githubusercontent.com/104444213/174568920-28c05f65-0f91-4390-8e2d-a77d835cdfbd.png)


Delete Config Lambda = delete_config
•	For the config passed in, delete or disable the Config configuration.
•	Log and return error and send SNS notification if delete is not successful.

![Copy of Copy of AWS Solution Architect-Associate (3)](https://user-images.githubusercontent.com/104444213/174569395-c6a70a29-36f9-474f-b12d-79c86d96fad5.png)
