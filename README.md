# CV 2020 SQL Camera List
SQL script to pull list of cameras in use with Salient CompleteView 2020 software

Name:       CompleteView 2020 Camera List
Purpose:    Produces a report of all cameras in the CompleteView database and their associated make, model, IP address, and MAC address
Author:     James Anderson
Date:       19May2020
Version:    1.3
Comments:   Cameras with multiple channels will have their own line item but share the same IP address; the first entry for that camera, regardless of channel count, may be the only camera to possess the MAC address information, but this isn't always the case

Version History:
 -  :		(16Apr2020) 1.0 Initial testing of code and assignment of column names
 -  :		(17Apr2020) 1.1 Added Make and Model columns to query
 -  :		(27Apr2020) 1.2 Added # of Channels, Channel ID, and MAC Address columns to query, changed Name to "CompleteView 2020 Camera List," updated Purpose, and added Comment regarding MAC Address records
 -  :		(19May2020) 1.3 Changed v.IsDeleted to c.IsDeleted to create a cleaner list of cameras that are not deleted