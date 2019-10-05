---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1692db39e581943b4d063994bb14ac626558108
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402702"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = true;

graphClient.me()
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```