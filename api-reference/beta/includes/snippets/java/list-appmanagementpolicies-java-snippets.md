---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb313347d507109268270400b24ab821945e2c60
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258926"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppManagementPolicyCollectionPage appManagementPolicies = graphClient.policies().appManagementPolicies()
    .buildRequest()
    .get();

```