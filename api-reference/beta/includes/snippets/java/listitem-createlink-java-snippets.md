---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b32f665ab6d3a168d2d0820d2744e3d6930eff2
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992386"
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