---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49cb1d4c41715a66d54a79cb7c0efc5f1e726408
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768914"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().termsOfUse().agreements("093b947f-8363-4979-a47d-4c52b33ee1be")
    .buildRequest()
    .delete();

```