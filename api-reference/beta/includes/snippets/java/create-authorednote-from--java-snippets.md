---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc68bd46ba9ff9cb59110ac0df018732c1e4a261
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561820"
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