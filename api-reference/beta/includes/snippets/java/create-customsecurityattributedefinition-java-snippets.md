---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17917a6095fd2857bbec51125616f034bffe44ac
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226787"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomSecurityAttributeDefinition customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition();
customSecurityAttributeDefinition.attributeSet = "Engineering";
customSecurityAttributeDefinition.description = "Target completion date";
customSecurityAttributeDefinition.isCollection = false;
customSecurityAttributeDefinition.isSearchable = true;
customSecurityAttributeDefinition.name = "ProjectDate";
customSecurityAttributeDefinition.status = "Available";
customSecurityAttributeDefinition.type = "String";
customSecurityAttributeDefinition.usePreDefinedValuesOnly = false;

graphClient.directory().customSecurityAttributeDefinitions()
    .buildRequest()
    .post(customSecurityAttributeDefinition);

```