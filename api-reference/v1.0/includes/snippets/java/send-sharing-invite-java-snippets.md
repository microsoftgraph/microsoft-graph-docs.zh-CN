---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f417dd34a934b41bcbf2d9148267fa48f26a764
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771028"
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
    .invite(requireSignIn,rolesList,sendInvitation,message,recipientsList,null,null)
    .buildRequest()
    .post();

```