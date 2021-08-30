---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d6608fc9d3ae2b318df25b88b1411c367c1192d5c3a73e9872588b57fd03368
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163621"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMemberCollectionPage members = graphClient.teams("ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062").members()
    .buildRequest()
    .filter("roles/any(r:r eq 'owner')")
    .get();

```