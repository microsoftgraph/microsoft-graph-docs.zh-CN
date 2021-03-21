---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec300038577c2729e02f8f54f56b117fd088ac83
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980464"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicy activityBasedTimeoutPolicy = graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .get();

```