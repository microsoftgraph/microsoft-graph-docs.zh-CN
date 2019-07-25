---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ee78f8abc323034bfe6c66208dc5fdac281016cb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855903"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReview accessReview = new AccessReview();
accessReview.displayName = "TestReview new name";

graphClient.accessReviews("006111db-0810-4494-a6df-904d368bd81b")
    .buildRequest()
    .patch(accessReview);

```