---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05862c1ecf3b5fcc6b5faeb84c98d67574dfdcf0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956712"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
conversationMember.roles = rolesList;

graphClient.teams("{id}").channels("{id}").members("{id}")
    .buildRequest()
    .patch(conversationMember);

```