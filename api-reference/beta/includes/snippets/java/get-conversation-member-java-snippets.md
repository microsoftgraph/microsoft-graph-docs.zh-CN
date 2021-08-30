---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c547b1f242363bab0ed497b20c2aec85d8d5e48cc480f905f854522fe544ce9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161286"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMember conversationMember = graphClient.chats("19:b8577894a63548969c5c92bb9c80c5e1@thread.v2").members("MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiODU3Nzg5NGE2MzU0ODk2OWM1YzkyYmI5YzgwYzVlMUB0aHJlYWQudjIjIzJjOGQyYjVjLTE4NDktNDA2Ni1iNTdkLWU3YTBlOWU0NGVjOA==")
    .buildRequest()
    .get();

```