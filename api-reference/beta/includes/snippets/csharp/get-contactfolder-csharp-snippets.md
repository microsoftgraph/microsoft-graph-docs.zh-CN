---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a5e204fd8c5f71e1b0d8a704b744d4fded7911a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = await graphClient.Me.ContactFolders["{contactFolder-id}"]
    .Request()
    .GetAsync();

```