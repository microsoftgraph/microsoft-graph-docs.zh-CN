---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec505595850dd2c3311748f5205ae9cb0533deccbe0feffdd6d4f0f4bd8d9bac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902662"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = graphClient.identityGovernance().accessReviews().definitions("5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0").instances("6444d4fd-ab55-4608-8cf9-c6702d172bcc").decisions("e6cafba0-cbf0-4748-8868-0810c7f4cc06")
    .buildRequest()
    .get();

```