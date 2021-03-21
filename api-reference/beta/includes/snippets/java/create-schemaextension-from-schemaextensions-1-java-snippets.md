---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b94dad46a96ac85261dcc8686a936b4880f8089
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968921"
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