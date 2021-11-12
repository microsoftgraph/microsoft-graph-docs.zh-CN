---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 612c4a0aec91dd2d788e82c8c1c803e10117fd712041ff599be7d56989b2693b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329038"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "embed";

graphClient.sites("{siteId}").lists("{listId}").items("{itemId}")
    .createLink(ListItemCreateLinkParameterSet
        .newBuilder()
        .withType(type)
        .withScope(null)
        .withExpirationDateTime(null)
        .withPassword(null)
        .withRecipients(null)
        .build())
    .buildRequest()
    .post();

```