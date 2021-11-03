---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc68bd46ba9ff9cb59110ac0df018732c1e4a261
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696346"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthoredNote authoredNote = new AuthoredNote();
ItemBody content = new ItemBody();
content.content = "String";
content.contentType = BodyType.TEXT;
authoredNote.content = content1;

graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}").notes()
    .buildRequest()
    .post(authoredNote);

```