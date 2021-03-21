---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abef2b3b46231c2d51383f01def91bddda289a7f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972145"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApprovalMyRequestsCollectionPage myRequests = graphClient.privilegedApproval()
    .myRequests()
    .buildRequest()
    .get();

```