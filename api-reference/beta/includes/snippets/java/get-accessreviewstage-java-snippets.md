---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf11dc0fa20f1df7d7987bb6e2a598c1a0e67a1f
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853343"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewStage accessReviewStage = graphClient.identityGovernance().accessReviews().definitions("6af553ce-104d-4842-ab5f-67d7b556e9dd").instances("9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24").stages("839ecbd4-ba5d-4d32-8249-e734aac47adf")
    .buildRequest()
    .get();

```