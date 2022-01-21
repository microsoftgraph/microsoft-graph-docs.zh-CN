---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 006fcde4ec2986b8fe40f79df5a4f6fca29e2dcf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137698"
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
        .withRetainInheritedPermissions(null)
        .build())
    .buildRequest()
    .post();

```