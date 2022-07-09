---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31940ce24dc92309e3fc80cb24c7c220cf5257b7
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853269"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("2b83cc42-09db-46f6-8c6e-16fec466a82d").instances("61a617dd-238f-4037-8fa5-d800e515f5bc").stages("5d431f4b-56f2-4a50-938b-fb1e4e2c91b9")
    .stop()
    .buildRequest()
    .post();

```