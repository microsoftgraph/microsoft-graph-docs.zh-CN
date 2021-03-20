---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e0b7e4fb58a9a760bc39071592fcc51088c565f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974566"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
conversationMember.roles = rolesList;

graphClient.teams("{id}").channels("{id}").members("{id}")
    .buildRequest()
    .patch(conversationMember);

```