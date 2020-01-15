---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1793de8aa4b815ce8722cabd68fdeebe03df5296
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123122"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerTaskCollectionPage tasks = graphClient.planner().buckets("{bucket-id}").tasks()
    .buildRequest()
    .get();

```