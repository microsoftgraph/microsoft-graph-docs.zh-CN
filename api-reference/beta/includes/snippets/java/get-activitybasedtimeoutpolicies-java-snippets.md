---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d59696062e49e56b115324529fd8633d5ff27ab9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973462"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicyCollectionPage activityBasedTimeoutPolicies = graphClient.policies().activityBasedTimeoutPolicies()
    .buildRequest()
    .get();

```