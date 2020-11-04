---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2ae0a0fc9b019298ef00fdca2e742c56bf50378
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905012"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$skiptoken", "c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA="));

ChatMessage chatMessage = graphClient.teams("{id}").channels("{id}").messages("delta")
    .buildRequest( requestOptions )
    .get();

```