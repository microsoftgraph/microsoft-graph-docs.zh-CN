---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0235bad8907e533066a39df878b4f2aa0c6379fd
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppManagementPolicy appManagementPolicy = new AppManagementPolicy();
appManagementPolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}"));

graphClient.applications("{id}").appManagementPolicies().references()
    .buildRequest()
    .post(appManagementPolicy);

```