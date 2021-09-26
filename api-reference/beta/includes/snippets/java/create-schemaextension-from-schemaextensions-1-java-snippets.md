---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e405394a763bef0606dfcdd0bddebcb3323d04ed0cdc69ebe862cab0ba70fdb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103957"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtension schemaExtension = new SchemaExtension();
schemaExtension.id = "graphlearn_courses";
schemaExtension.description = "Graph Learn training courses extensions";
LinkedList<String> targetTypesList = new LinkedList<String>();
targetTypesList.add("Group");
schemaExtension.targetTypes = targetTypesList;
LinkedList<ExtensionSchemaProperty> propertiesList = new LinkedList<ExtensionSchemaProperty>();
ExtensionSchemaProperty properties = new ExtensionSchemaProperty();
properties.name = "courseId";
properties.type = "Integer";
propertiesList.add(properties);
ExtensionSchemaProperty properties1 = new ExtensionSchemaProperty();
properties1.name = "courseName";
properties1.type = "String";
propertiesList.add(properties1);
ExtensionSchemaProperty properties2 = new ExtensionSchemaProperty();
properties2.name = "courseType";
properties2.type = "String";
propertiesList.add(properties2);
schemaExtension.properties = propertiesList;

graphClient.schemaExtensions()
    .buildRequest()
    .post(schemaExtension);

```