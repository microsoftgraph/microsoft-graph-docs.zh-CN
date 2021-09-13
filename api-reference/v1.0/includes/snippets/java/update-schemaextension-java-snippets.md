---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13b63658980c7fdb83cb3a1b25f3ed4e69b9995763ddf85e66b1afa41ffaaa8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274208"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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