---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0c2fa5bf80eccb53e10ac8d0afb82ba0f7d5b75
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805603"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .delete();

```