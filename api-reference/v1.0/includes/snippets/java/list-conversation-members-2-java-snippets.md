---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5f23df22d0a75dfe5cda5ee55155a4d7d25c526
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202348"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMemberCollectionPage members = graphClient.chats("{id}").members()
    .buildRequest()
    .get();

```