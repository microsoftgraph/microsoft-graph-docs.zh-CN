---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4203d7843bb4e46ab9e7b8a0a312126ee12a4628
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970638"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReviewSetQuery reviewSetQuery = new ReviewSetQuery();
reviewSetQuery.displayName = "My Query 1";
reviewSetQuery.query = "(subject:\"Quarterly Financials\")";

graphClient.compliance().ediscovery().cases("2eef613a-ca2d-42f4-89fe-84d5198ddedf").reviewSets("b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8").queries()
    .buildRequest()
    .post(reviewSetQuery);

```