---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f0bcd6a29e98d973068cad83995d5267ffce84d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974082"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .delete();

```