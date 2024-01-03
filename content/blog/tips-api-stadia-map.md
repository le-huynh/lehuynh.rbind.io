+++
showonlyimage = false
draft = false
image = "img/tips.png"
title = "Getting Stadia Maps API for ggmap Rpackage"
weight = 2
description = " "
+++

The *ggmap* R package is a powerful tool for creating stunning map visualizations in R, making mapping tasks more accessible and efficient. 
To enable Stadia Maps services in R, an API key is required. 
A free API key for non-commercial use can be obtained without requiring a credit card for sign-up. 

#### Obtain and set API key for R session 
1. Sign up for Stadia Maps at https://client.stadiamaps.com/signup/

2. Navigate to the client dashboard at https://client.stadiamaps.com/dashboard/

3. Click on **Create a Property** → insert **Property Name** → click on **Create**

4. Under **Authentication Configuration**, select **Add API key**

5. Copy the provided API key and execute the following code in the console


```
ggmap::register_stadiamaps(key = "YOUR-API-KEY", write = FALSE)
```

When setting the API key:
- Using `write = FALSE` to configure the key for the current R session only. The API key needs to be provided again when restarting R.
- Using `write = TRUE` to set the API key permanently across R sessions.

```
Note: The API key is a PRIVATE access key and should be handled with caution. 
Avoid sharing it online, like in a public GitHub repository, or storing it in a shared R script file.
```

6. If the API key is shared inadvertently, access https://client.stadiamaps.com/ → delete the existing API key → generate a new one

#### Further information
- [Authentication](https://docs.stadiamaps.com/authentication/#api-keys) by Stadia Maps Documentation
- [*ggmap* Documentation](https://www.rdocumentation.org/packages/ggmap/versions/4.0.0)




