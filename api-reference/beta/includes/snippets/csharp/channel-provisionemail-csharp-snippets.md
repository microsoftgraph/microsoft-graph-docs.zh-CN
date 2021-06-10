---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca53dfaae351f3e574313c7bdc3218229df09b42
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869643"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .ProvisionEmail()
    .Request()
    .PostAsync();

```