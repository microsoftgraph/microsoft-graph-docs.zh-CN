---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6ef3ce7ba71edb026b6a8e10307ac3ae4bea05ca9b83a200c2ae9778c3c05e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218866"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMemberCollectionPage members = graphClient.teams("ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062").members()
    .buildRequest()
    .get();

```