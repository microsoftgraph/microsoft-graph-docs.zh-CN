---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaabff56dc602d6a59adb183a139068fda96beb7
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780510"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')"));

graphClient.policies().mobileAppManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020").includedGroups().references()
    .buildRequest()
    .post(group);

```