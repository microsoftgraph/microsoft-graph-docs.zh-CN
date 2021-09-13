---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0edbd5f38ae956d6f220c26426bc9f33007a47b73de2173533bcb311a23e21b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274276"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContentCollectionPage hostedContents = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages("1616963377068").replies("1616963389737").hostedContents()
    .buildRequest()
    .get();

```