---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58146d0027f408732cce6d3a5b521261df0ab3d463b77896740d68f6b6ca3d23
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219919"
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