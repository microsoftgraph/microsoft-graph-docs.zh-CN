---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f018ab24369730948c940362b8167aec09be9876
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977010"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().buckets("gcrYAaAkgU2EQUvpkNNXLGQAGTtu").tasks()
    .buildRequest()
    .get();

```