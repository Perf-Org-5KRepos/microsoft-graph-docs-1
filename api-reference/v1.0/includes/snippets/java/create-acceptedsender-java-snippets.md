---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "alexd@contoso.com";

graphClient.groups("{id}").acceptedSenders().references()
	.buildRequest()
	.post(directoryObject);

```