---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: caabd73511946ec0ad1afbc052d83d448657ca0d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348792"
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
        .withExpirationDateTime(expirationDateTime)
        .withPassword(password)
        .build())
    .buildRequest()
    .post();

```