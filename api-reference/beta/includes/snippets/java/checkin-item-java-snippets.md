---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1d00bb9a7d6a42d6924a7a0ef9215e8e08ff93ecde41b3bb0775b261513399e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278403"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "Updating the latest guidelines";

graphClient.drives("{drive-id}").items("{item-id}")
    .checkin(DriveItemCheckinParameterSet
        .newBuilder()
        .withCheckInAs(null)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```