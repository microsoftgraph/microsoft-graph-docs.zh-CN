---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50ddcc52798724046b61d2a7e185b2d8dcdbe60d
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854108"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItemCollectionPage decisions = graphClient.identityGovernance().accessReviews().definitions("16d424f6-0100-4bf1-9ebc-fe009c5e5006").instances("bb14c722-51b8-4962-9bd2-1d96ba773d80").stages("8f0a8999-205b-4c29-a68c-2bee353fd4c5").decisions()
    .buildRequest()
    .get();

```