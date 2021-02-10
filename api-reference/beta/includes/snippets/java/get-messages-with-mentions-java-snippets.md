---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 403dedef55ed3f28a3c9c662913194f4f509db3c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176991"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .filter("MentionsPreview/IsMentioned eq true")
    .select("subject,sender,receivedDateTime,mentionsPreview")
    .get();

```