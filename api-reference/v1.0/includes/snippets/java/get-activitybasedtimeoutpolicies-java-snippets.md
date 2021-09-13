---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91cb4b43a9487e4a5086afdd67d79357242a5fff7573a0367ffb91e19eeefd48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278628"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicyCollectionPage activityBasedTimeoutPolicies = graphClient.policies().activityBasedTimeoutPolicies()
    .buildRequest()
    .get();

```