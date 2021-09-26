---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93726e5cc206fef07ab631bcd451da4f4792ac2a
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767302"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtension schemaExtension = new SchemaExtension();
schemaExtension.owner = "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa";
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
ExtensionSchemaProperty properties3 = new ExtensionSchemaProperty();
properties3.name = "courseSupervisors";
properties3.type = "String";
propertiesList.add(properties3);
schemaExtension.properties = propertiesList;

graphClient.schemaExtensions("exto6x7sfft_courses")
    .buildRequest()
    .patch(schemaExtension);

```