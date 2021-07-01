---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c6797ef2a6c0a68cc4cf5830fec356fdc1d0108
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209902"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances("1234fba0-cbf0-5678-8868-0810c7f49101")
    .applyDecisions()
    .buildRequest()
    .post();

```