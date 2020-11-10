---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fa8da061df043c019c8eba88a56c8f255b170bb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970015"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemGetActivitiesByIntervalCollectionPage getActivitiesByInterval = graphClient.drives("{drive-id}").items("{item-id}")
    .getActivitiesByInterval("2017-01-01","2017-01-3","day")
    .buildRequest()
    .get();

```