---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 243ae4043c897305351ebb4568149945d51deed9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972733"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .filter("MentionsPreview/IsMentioned eq true")
    .select("subject,sender,receivedDateTime,mentionsPreview")
    .get();

```