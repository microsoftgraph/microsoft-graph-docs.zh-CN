---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bead0dae0519f291faec5613789a25828c0bb52
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610380"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContentCollectionPage hostedContents = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages("1616963377068").replies("1616963389737").hostedContents()
    .buildRequest()
    .get();

```