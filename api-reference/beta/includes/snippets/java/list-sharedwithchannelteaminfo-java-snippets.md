---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 584f0ccb139846d5abab8de577cbee42dc306011
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212795"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SharedWithChannelTeamInfoCollectionPage sharedWithTeams = graphClient.teams("893075dd-2487-4122-925f-022c42e20265").channels("19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2").sharedWithTeams()
    .buildRequest()
    .get();

```