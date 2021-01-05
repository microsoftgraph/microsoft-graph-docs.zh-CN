---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f3b077f2ce6ce3229315bd0185ae95c913f2a70
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["8b081ef6-4792-4def-b2c9-c363a1bf41d5"].Chats["19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces"]
    .Request()
    .GetAsync();

```