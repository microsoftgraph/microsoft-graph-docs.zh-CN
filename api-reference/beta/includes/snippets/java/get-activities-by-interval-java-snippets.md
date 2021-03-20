---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 544454a4072f74e34438c9039c409a59735cc03f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978651"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemGetActivitiesByIntervalCollectionPage getActivitiesByInterval = graphClient.drives("{drive-id}").items("{item-id}")
    .getActivitiesByInterval(DriveItemGetActivitiesByIntervalParameterSet
        .newBuilder()
        .withStartDateTime("2017-01-01")
        .withEndDateTime("2017-01-3")
        .withInterval("day")
        .build())
    .buildRequest()
    .get();

```