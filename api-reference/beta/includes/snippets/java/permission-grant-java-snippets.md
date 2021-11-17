---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40276f497caff025d055a915a019863dbf5121193a25a21cebb34f15c4be8b84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215804"
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