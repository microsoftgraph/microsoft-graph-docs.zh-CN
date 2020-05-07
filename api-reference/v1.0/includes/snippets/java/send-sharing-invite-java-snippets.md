---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93349ba8daf182141daa87bad6e3f30672e18610
ms.sourcegitcommit: df2c52f84aae5d4fed641d7411ba547371f0eaad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2020
ms.locfileid: "44055602"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();
recipients.email = "ryan@contoso.com";

recipientsList.add(recipients);

String message = "Here's the file that we're collaborating on.";

boolean requireSignIn = true;

boolean sendInvitation = true;

LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("write");

String password = "password123";

int expirationDateTime = 7/15/2018 2:00:00 PM;

graphClient.me().drive().items("{item-id}")
    .invite(requireSignIn,rolesList,sendInvitation,message,recipientsList,expirationDateTime,password)
    .buildRequest()
    .post();

```