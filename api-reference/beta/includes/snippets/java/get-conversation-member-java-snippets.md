---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5b8acd99cc7ae5430e21e5e579ecc5beb91f2dc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862965"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConversationMemberCollectionPage members = graphClient.me().chats("{id}").members()
    .buildRequest()
    .get();

```