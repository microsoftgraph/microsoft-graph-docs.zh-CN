---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 386c118504141b7bc1b1dde4cbdaabd2b6b9651e
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931628"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .grant(rolesList,recipientsList)
    .buildRequest()
    .post();

```