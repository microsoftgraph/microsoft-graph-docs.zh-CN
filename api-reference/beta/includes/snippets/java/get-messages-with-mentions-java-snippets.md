---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 658ce92e118d0fed7e242a1cd2820ceebb29dfe1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975309"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .filter("MentionsPreview/IsMentioned eq true,")
    .select("subject,sender,receivedDateTime,mentionsPreview")
    .get();

```