---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bd39a987e6fc22d17943adcd3ba0f9283ee3ed9
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314501"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConversationMemberCollectionPage members = graphClient.teams("{teamsId}").members()
    .buildRequest()
    .get();

```