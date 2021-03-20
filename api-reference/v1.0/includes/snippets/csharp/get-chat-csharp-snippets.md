---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa6206a48d75e93bedc7b433b5ed1056f878106d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950131"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var spaces = await graphClient.Users["{user-id}"].Chats.19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces
    .Request()
    .GetAsync();

```