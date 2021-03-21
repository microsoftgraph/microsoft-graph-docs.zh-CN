---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 798a6a54fa6b371eec26dc32aff971853e982748
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982184"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMemberCollectionPage members = graphClient.teams("ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062").members()
    .buildRequest()
    .filter("roles/any(r:r eq 'owner')")
    .get();

```