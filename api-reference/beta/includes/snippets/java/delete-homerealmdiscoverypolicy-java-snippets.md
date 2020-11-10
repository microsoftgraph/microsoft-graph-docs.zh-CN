---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0c2fa5bf80eccb53e10ac8d0afb82ba0f7d5b75
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964795"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .delete();

```