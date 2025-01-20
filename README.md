Text Retrieval: You retrieved text from an S3 bucket (aws-pj-1) using s3.get_object.

Polly Synthesis: You sent the text to Amazon Polly to synthesize speech. Polly converted the text into an audio stream in MP3 format.

Stream Handling: The audio stream was read and stored as a byte array to avoid the seek error when uploading to S3.

S3 Upload: The audio byte array was uploaded back to S3 as an MP3 file with a unique name.
