---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aad025b6aee751eff15c13eaf8c7696230fe2798
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTab teamsTab = graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").tabs("d731fca0-0f14-4537-971a-0ef9101ff13d")
    .buildRequest()
    .expand("teamsApp")
    .get();

```