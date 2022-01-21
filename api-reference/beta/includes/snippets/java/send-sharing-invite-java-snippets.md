---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 077bbbcaa10384dfc44989e862838dcbcfb910b7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137639"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();
recipients.email = "robin@contoso.org";

recipientsList.add(recipients);

String message = "Here's the file that we're collaborating on.";

Boolean requireSignIn = true;

Boolean sendInvitation = true;

LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("write");

String password = "password123";

String expirationDateTime = "07/15/2018 14:00:00";

graphClient.me().drive().items("{item-id}")
    .invite(DriveItemInviteParameterSet
        .newBuilder()
        .withRequireSignIn(requireSignIn)
        .withRoles(rolesList)
        .withSendInvitation(sendInvitation)
        .withMessage(message)
        .withRecipients(recipientsList)
        .withRetainInheritedPermissions(null)
        .withExpirationDateTime(expirationDateTime)
        .withPassword(password)
        .build())
    .buildRequest()
    .post();

```