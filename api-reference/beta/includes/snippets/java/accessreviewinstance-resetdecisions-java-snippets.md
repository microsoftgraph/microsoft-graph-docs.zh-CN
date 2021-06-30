---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56bd2e43718ff6949491c0b3054475317f84911d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207523"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("0185aab8-9a7e-44b5-ae36-41b923c3bf87").instances("1234aab8-9a7e-44b5-ae36-41b923c3bf87")
    .resetDecisions()
    .buildRequest()
    .post();

```