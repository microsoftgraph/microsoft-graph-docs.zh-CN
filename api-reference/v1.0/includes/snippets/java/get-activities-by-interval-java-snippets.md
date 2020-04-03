---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae852a2292e38e925c0b3b1b44a7e2e3ddfb3248
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124859"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IItemActivityStatCollectionPage getActivitiesByInterval = graphClient.drives("{drive-id}").items("{item-id}")
    .getActivitiesByInterval("2017-01-01","2017-01-3","day")
    .buildRequest()
    .get();

```