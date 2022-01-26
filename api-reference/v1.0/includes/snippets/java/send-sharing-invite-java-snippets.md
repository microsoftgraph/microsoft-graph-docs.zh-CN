---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03980e2b9f5f72afddcc4e761feff3528addcf6d
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62227527"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();
recipients.email = "ryan@contoso.com";

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