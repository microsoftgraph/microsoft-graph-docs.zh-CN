---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6c5dd393054daf94b8777ff06368b97f070c481
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951582"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewDecisionCollectionPage myDecisions = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").myDecisions()
    .buildRequest()
    .get();

```