---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7257c4660d74861f080c05525c01f213f5107f3e9e439e73e4ac61157aeb3395
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105487"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .filter("MentionsPreview/IsMentioned eq true")
    .select("subject,sender,receivedDateTime,mentionsPreview")
    .get();

```