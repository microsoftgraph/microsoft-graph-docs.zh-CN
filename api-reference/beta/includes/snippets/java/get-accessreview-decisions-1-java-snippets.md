---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bdf0100fc25eec6b4db67f93b5e836a9df3c997
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943166"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewDecisionCollectionPage decisions = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").decisions()
    .buildRequest()
    .get();

```