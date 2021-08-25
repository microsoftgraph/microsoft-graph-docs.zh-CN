---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37e41144adc9ae694ab4272e1cf032327dfdb9a0
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516043"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schema schema = new Schema();
schema.baseType = "microsoft.graph.externalItem";
LinkedList<Property> propertiesList = new LinkedList<Property>();
Property properties = new Property();
properties.name = "ticketTitle";
properties.type = PropertyType.STRING;
properties.isSearchable = false;
properties.isRetrievable = false;
LinkedList<Label> labelsList = new LinkedList<Label>();
labelsList.add(Label.TITLE);
properties.labels = labelsList;
propertiesList.add(properties);
Property properties1 = new Property();
properties1.name = "priority";
properties1.type = PropertyType.STRING;
properties1.isQueryable = false;
properties1.isRetrievable = false;
properties1.isSearchable = false;
propertiesList.add(properties1);
Property properties2 = new Property();
properties2.name = "assignee";
properties2.type = PropertyType.STRING;
properties2.isRetrievable = false;
propertiesList.add(properties2);
schema.properties = propertiesList;

graphClient.external().connections("contosohr").schema()
    .buildRequest()
    .post(schema);

```