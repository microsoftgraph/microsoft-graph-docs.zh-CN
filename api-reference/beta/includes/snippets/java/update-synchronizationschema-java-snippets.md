---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b8e6eafbc7d339941b7000ec3c7d0cfe2d583b3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974038"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationSchema synchronizationSchema = new SynchronizationSchema();
LinkedList<DirectoryDefinition> directoriesList = new LinkedList<DirectoryDefinition>();
DirectoryDefinition directories = new DirectoryDefinition();
directories.name = "Azure Active Directory";
LinkedList<ObjectDefinition> objectsList = new LinkedList<ObjectDefinition>();
ObjectDefinition objects = new ObjectDefinition();
objects.name = "User";
LinkedList<AttributeDefinition> attributesList = new LinkedList<AttributeDefinition>();
AttributeDefinition attributes = new AttributeDefinition();
attributes.name = "userPrincipalName";
attributes.type = AttributeType.STRING;
attributesList.add(attributes);
objects.attributes = attributesList;
objectsList.add(objects);
directories.objects = objectsList;
directoriesList.add(directories);
DirectoryDefinition directories1 = new DirectoryDefinition();
directories1.name = "Salesforce";
directoriesList.add(directories1);
DirectoryDefinitionCollectionResponse directoryDefinitionCollectionResponse = new DirectoryDefinitionCollectionResponse();
directoryDefinitionCollectionResponse.value = directoriesList;
DirectoryDefinitionCollectionPage directoryDefinitionCollectionPage = new DirectoryDefinitionCollectionPage(directoryDefinitionCollectionResponse, null);
synchronizationSchema.directories = directoryDefinitionCollectionPage;
LinkedList<SynchronizationRule> synchronizationRulesList = new LinkedList<SynchronizationRule>();
SynchronizationRule synchronizationRules = new SynchronizationRule();
synchronizationRules.name = "USER_TO_USER";
synchronizationRules.sourceDirectoryName = "Azure Active Directory";
synchronizationRules.targetDirectoryName = "Salesforce";
LinkedList<ObjectMapping> objectMappingsList = new LinkedList<ObjectMapping>();
ObjectMapping objectMappings = new ObjectMapping();
objectMappings.sourceObjectName = "User";
objectMappings.targetObjectName = "User";
LinkedList<AttributeMapping> attributeMappingsList = new LinkedList<AttributeMapping>();
AttributeMapping attributeMappings = new AttributeMapping();
AttributeMappingSource source = new AttributeMappingSource();
attributeMappings.source = source;
attributeMappings.targetAttributeName = "userName";
attributeMappingsList.add(attributeMappings);
objectMappings.attributeMappings = attributeMappingsList;
objectMappingsList.add(objectMappings);
synchronizationRules.objectMappings = objectMappingsList;
synchronizationRulesList.add(synchronizationRules);
synchronizationSchema.synchronizationRules = synchronizationRulesList;

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .buildRequest()
    .put(synchronizationSchema);

```