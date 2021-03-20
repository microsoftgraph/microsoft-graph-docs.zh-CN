---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7220a1fd72fd91bb44e926f7140a397f64d82978
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978057"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();
recipients.email = "ryan@contoso.org";

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