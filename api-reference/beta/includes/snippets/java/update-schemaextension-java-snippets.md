---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a8228e07c9da540665615b98064712514a44cc0d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870582"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtension schemaExtension = new SchemaExtension();
LinkedList<ExtensionSchemaProperty> propertiesList = new LinkedList<ExtensionSchemaProperty>();
ExtensionSchemaProperty properties = new ExtensionSchemaProperty();
properties.name = "new-name-value";
properties.type = "new-type-value";
propertiesList.add(properties);
ExtensionSchemaProperty properties1 = new ExtensionSchemaProperty();
properties1.name = "additional-name-value";
properties1.type = "additional-type-value";
propertiesList.add(properties1);
schemaExtension.properties = propertiesList;

graphClient.schemaExtensions("{id}")
    .buildRequest()
    .patch(schemaExtension);

```