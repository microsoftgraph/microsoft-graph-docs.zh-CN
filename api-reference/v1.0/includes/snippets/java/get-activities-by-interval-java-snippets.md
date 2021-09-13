---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b67568a6d5ea99b1d8b19bac9aa72c874bf4d0bbd040e7dfe1c5d0dbbc89b369
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104968"
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