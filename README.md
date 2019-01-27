# Parity Cube Pvt Ltd (Assignment).
=> Image Sharing App

Ruby version - 2.6.0
Rails verion - 5.2.1

# Description
-> Firstly, Users has to sign up on the website via their email address and password.

-> Now user can able to create their own personal albums by clicking on the New Album button.

-> Can upload up to 25 images per album at once. (Users can create any number of albums).

-> Images uploaded by users would be listed on the homepage. All users/visitors can browse any album.

-> A user can be able to update album properties by clicking on edit button and also can able to see 
   particular album by clicking on show button.

-> My Albums page will display all the albums of the particular user.

# gems
# devise - Authentication

-> Devise is a flexible authentication solution for Rails based on Warden. It:

Is Rack based;
Is a complete MVC solution based on Rails engines;
Allows you to have multiple models signed in at the same time;
Is based on a modularity concept: use only what you really need.

# mini_magick - Resizing Image

-> Using MiniMagick the ruby processes memory remains small (it spawns ImageMagick's command line program mogrify which takes up some memory as well, but is much smaller compared to RMagick)

# Dependency
ImageMagick on server/system

# Concept
Active Storage

-> Active Storage is a built-in gem included on Rails 5.2 that handles file uploads to storage services from Amazon, Google, and Microsoft. Saving to local disk is also possible for development and test environments.

-> A migration is also created automatically for new applications. If you want to copy the migrations manually, run
  :bin/rails active_storage:install:migrations
  :bin/rails db:migrate
This migration adds two tables - active_storage_blobs and active_storage_attachments. These are for the 2 models Blob and Attachment. Blob stores metadata like filename, content-type, byte size and checksum. The actual file is stored in the storage service or disk depending on your settings.

A Blob can be attached to one or more Active Record objects through the Attachment join model.

# Routes
/albums - Home Page with 25 latest Galleries.
/my_gallery - User page with all his galleries.
