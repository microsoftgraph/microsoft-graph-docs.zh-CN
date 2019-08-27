---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0023d2a430b9edda902b8e22ad49161b82cc528
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Me.Chats["{id}"].Members
    .Request()
    .GetAsync();

```