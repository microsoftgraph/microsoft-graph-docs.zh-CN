---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6df14537a7fcce0236cf3837a1c12381c6f91a86
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952514"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IActivityBasedTimeoutPolicyCollectionPage activityBasedTimeoutPolicies = graphClient.policies().activityBasedTimeoutPolicies()
    .buildRequest()
    .get();

```