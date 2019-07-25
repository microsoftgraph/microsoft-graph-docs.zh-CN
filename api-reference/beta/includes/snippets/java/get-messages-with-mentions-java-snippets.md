---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cca8914c9dca75380ecf4087e1d318c29790b6ca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867198"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "MentionsPreview/IsMentioned eq true,"));

IMessageCollectionPage messages = graphClient.me().messages()
    .buildRequest( requestOptions )
    .select("subject,sender,receivedDateTime,mentionsPreview")
    .get();

```