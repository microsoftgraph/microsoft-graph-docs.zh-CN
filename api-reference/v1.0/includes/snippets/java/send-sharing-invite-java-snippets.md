---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c5a10716640de706b8e52849c84fcf31ff4aa1e
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402801"
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

graphClient.me().drive().items("{item-id}")
    .invite(requireSignIn,rolesList,sendInvitation,message,recipientsList)
    .buildRequest()
    .post();

```