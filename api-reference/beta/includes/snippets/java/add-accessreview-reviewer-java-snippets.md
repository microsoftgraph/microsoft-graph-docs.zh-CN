---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc1f4d0795d240fe0f6be4ccdcfc625e2aa42325c52496514d0aa24aeb04d245
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104165"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewReviewer accessReviewReviewer = new AccessReviewReviewer();
accessReviewReviewer.id = "006111db-0810-4494-a6df-904d368bd81b";

graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").reviewers()
    .buildRequest()
    .post(accessReviewReviewer);

```