---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 442798dcebf4a3c70a471269cb1ac006ff3b0393
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971660"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerBucketCollectionPage buckets = graphClient.planner().plans("2txjA-BMZEq-bKi6Wfj5aGQAB1OJ").buckets()
    .buildRequest()
    .get();

```