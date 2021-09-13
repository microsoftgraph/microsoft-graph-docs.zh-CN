---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5da76860c731e83a1cd65617bd4dfa0c833ae8ee3078073469c58c33c791da67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378884"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstance accessReviewInstance = graphClient.identityGovernance().accessReviews().definitions("e6cafba0-cbf0-4748-8868-0810c7f4cc06").instances("12345ba0-cbf0-5678-8868-4444c7f4cc06")
    .buildRequest()
    .get();

```