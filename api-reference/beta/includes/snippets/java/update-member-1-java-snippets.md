---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3581470262b23c32ad6c0aa93348adc6741973f3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208647"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AadUserConversationMember conversationMember = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
conversationMember.roles = rolesList;

graphClient.teams("ece6f0a1-7ca4-498b-be79-edf6c8fc4d82").channels("19:56eb04e133944cf69e603c5dac2d292e@thread.skype").members("ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=")
    .buildRequest()
    .patch(conversationMember);

```