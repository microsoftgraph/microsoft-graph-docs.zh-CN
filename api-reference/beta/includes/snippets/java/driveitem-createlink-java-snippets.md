---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aec64c84812c5deb3504835a64a3498ead051507
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137749"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "view";

String scope = "anonymous";

String password = "String";

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();

recipientsList.add(recipients);

graphClient.me().drive().items("{itemId}")
    .createLink(DriveItemCreateLinkParameterSet
        .newBuilder()
        .withType(type)
        .withScope(scope)
        .withExpirationDateTime(null)
        .withPassword(password)
        .withMessage(null)
        .withRecipients(recipientsList)
        .withRetainInheritedPermissions(null)
        .build())
    .buildRequest()
    .post();

```