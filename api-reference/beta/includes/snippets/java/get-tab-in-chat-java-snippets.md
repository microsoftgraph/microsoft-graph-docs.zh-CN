---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11c2276a670d596d70ad24caf81e21217eb69749
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689995"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTab teamsTab = graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").tabs("d731fca0-0f14-4537-971a-0ef9101ff13d")
    .buildRequest()
    .expand("teamsApp")
    .get();

```