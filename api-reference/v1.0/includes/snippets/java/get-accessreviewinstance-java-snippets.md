---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43137c886f8c2209bf86277204779d11e2834a7a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210995"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstance accessReviewInstance = graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances("12345ba0-cbf0-5678-8868-4444c7f4cc06")
    .buildRequest()
    .get();

```