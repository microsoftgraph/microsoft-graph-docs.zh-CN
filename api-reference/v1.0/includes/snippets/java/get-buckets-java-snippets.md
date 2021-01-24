---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7514070d447b49e247cce8f82fee8c47182f8536
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945914"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerBucketCollectionPage buckets = graphClient.planner().buckets()
    .buildRequest()
    .get();

```