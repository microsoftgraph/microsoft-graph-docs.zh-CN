---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13dd0d6f6b5a9b66ad76711750ccb5cbcc2023d6
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611250"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContentCollectionPage hostedContents = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages("1616963377068").hostedContents()
    .buildRequest()
    .get();

```