---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b82b76be04a3dc4f88713d45080d7e71193b9140
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869105"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
synchronizationSchema.directories = directoriesList;
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