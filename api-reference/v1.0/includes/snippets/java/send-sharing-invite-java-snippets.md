---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 66f30ce9cb3af0f26eba320aec6aa8d734fd5c21
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890799"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();
recipients.email = "ryan@contoso.com";

recipientsList.add(recipients);

String message = "Here's the file that we're collaborating on.";

boolean requireSignIn = True;

boolean sendInvitation = True;

LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("write");

graphClient.me().drive().items("{item-id}")
    .invite(requireSignIn,rolesList,sendInvitation,message,recipientsList)
    .buildRequest()
    .post();

```