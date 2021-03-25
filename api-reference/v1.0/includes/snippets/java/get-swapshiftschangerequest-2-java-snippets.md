---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ceac2155914868c1ffc8b92cde14771b42754836
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210685"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SwapShiftsChangeRequestCollectionPage swapShiftsChangeRequests = graphClient.teams("{teamId}").schedule().swapShiftsChangeRequests()
    .buildRequest()
    .get();

```