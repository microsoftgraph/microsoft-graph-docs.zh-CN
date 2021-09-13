---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5ac83a4ff2d153378cf5b92117573d666d15c832f5847764ec2ce8d9cae6880
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106806"
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
        .withExpirationDateTime(expirationDateTime)
        .withPassword(password)
        .build())
    .buildRequest()
    .post();

```