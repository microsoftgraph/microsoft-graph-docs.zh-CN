---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e4902b319797c4a17f18b692e56a00e753cedff
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppManagementPolicy appManagementPolicy = new AppManagementPolicy();
appManagementPolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}"));

graphClient.servicePrincipals("{id}").appManagementPolicies().references()
    .buildRequest()
    .post(appManagementPolicy);

```