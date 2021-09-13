---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57ca2a633d8ec6f9b663bb0a379bdc664475efe8b8c96d1bc32ea9120a5ec479
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409585"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTab teamsTab = graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").tabs("d731fca0-0f14-4537-971a-0ef9101ff13d")
    .buildRequest()
    .expand("teamsApp")
    .get();

```