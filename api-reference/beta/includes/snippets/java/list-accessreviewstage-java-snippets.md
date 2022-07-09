---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27286e7e9b52000aa57887a5f36c33610c70fc06
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853780"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewStageCollectionPage stages = graphClient.identityGovernance().accessReviews().definitions("16d424f6-0100-4bf1-9ebc-fe009c5e5006").instances("bb14c722-51b8-4962-9bd2-1d96ba773d80").stages()
    .buildRequest()
    .get();

```