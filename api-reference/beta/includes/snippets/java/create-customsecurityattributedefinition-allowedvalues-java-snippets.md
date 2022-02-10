---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4680356b99834bd5d5fed98aebc104de834616d2
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519335"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomSecurityAttributeDefinition customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition();
customSecurityAttributeDefinition.attributeSet = "Engineering";
customSecurityAttributeDefinition.description = "Active projects for user";
customSecurityAttributeDefinition.isCollection = true;
customSecurityAttributeDefinition.isSearchable = true;
customSecurityAttributeDefinition.name = "Project";
customSecurityAttributeDefinition.status = "Available";
customSecurityAttributeDefinition.type = "String";
customSecurityAttributeDefinition.usePreDefinedValuesOnly = true;
LinkedList<AllowedValue> allowedValuesList = new LinkedList<AllowedValue>();
AllowedValue allowedValues = new AllowedValue();
allowedValues.id = "Alpine";
allowedValues.isActive = true;
allowedValuesList.add(allowedValues);
AllowedValue allowedValues1 = new AllowedValue();
allowedValues1.id = "Baker";
allowedValues1.isActive = true;
allowedValuesList.add(allowedValues1);
AllowedValue allowedValues2 = new AllowedValue();
allowedValues2.id = "Cascade";
allowedValues2.isActive = true;
allowedValuesList.add(allowedValues2);
AllowedValueCollectionResponse allowedValueCollectionResponse = new AllowedValueCollectionResponse();
allowedValueCollectionResponse.value = allowedValuesList;
AllowedValueCollectionPage allowedValueCollectionPage = new AllowedValueCollectionPage(allowedValueCollectionResponse, null);
customSecurityAttributeDefinition.allowedValues = allowedValueCollectionPage;

graphClient.directory().customSecurityAttributeDefinitions()
    .buildRequest()
    .post(customSecurityAttributeDefinition);

```