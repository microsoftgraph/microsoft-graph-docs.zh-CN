---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88c5b62131b09a238de685b92dd7238716f54201
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972658"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstance accessReviewInstance = graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-444404f3baa6").instances("12490cdb-6a18-4c08-ba2c-44442f0a0138")
    .buildRequest()
    .get();

```