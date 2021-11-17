---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7eb49e9e9d33e92d274f79a7eed1d9a187532c66ab79029450bd05b6ed656d79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902608"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicy activityBasedTimeoutPolicy = graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .get();

```