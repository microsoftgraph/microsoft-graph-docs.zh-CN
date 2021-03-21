---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 614f6ed6478b1cdfc388d9280a0cdcb61506c018
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973596"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();
recipients.email = "john@contoso.com";

recipientsList.add(recipients);
DriveRecipient recipients1 = new DriveRecipient();
recipients1.email = "ryan@external.com";

recipientsList.add(recipients1);

LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("read");

graphClient.shares("{encoded-sharing-url}").permission()
    .grant(PermissionGrantParameterSet
        .newBuilder()
        .withRoles(rolesList)
        .withRecipients(recipientsList)
        .build())
    .buildRequest()
    .post();

```