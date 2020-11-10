---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09b802ff5440ee62a5e5b5391e03f1e59ab24201
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964753"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IHomeRealmDiscoveryPolicyCollectionPage homeRealmDiscoveryPolicies = graphClient.policies().homeRealmDiscoveryPolicies()
    .buildRequest()
    .get();

```