---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 648466ed577915c6ea35cccae6ef33c13ecd4d92
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209062"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContent chatMessageHostedContent = graphClient.chats("{id}").messages("{id}").hostedContents("{id}")
    .buildRequest()
    .get();

```