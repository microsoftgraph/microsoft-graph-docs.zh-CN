---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 995da2f9b786e790f0e3fc91250ff4dc8074b64e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951701"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReview accessReview = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d")
    .buildRequest()
    .get();

```