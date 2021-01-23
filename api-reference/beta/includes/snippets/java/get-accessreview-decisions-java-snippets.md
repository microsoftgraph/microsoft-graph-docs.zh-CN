---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bdf0100fc25eec6b4db67f93b5e836a9df3c997
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946071"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessReviewDecisionCollectionPage decisions = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").decisions()
    .buildRequest()
    .get();

```