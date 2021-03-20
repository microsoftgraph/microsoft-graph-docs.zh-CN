---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7514070d447b49e247cce8f82fee8c47182f8536
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941545"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerBucketCollectionPage buckets = graphClient.planner().buckets()
    .buildRequest()
    .get();

```