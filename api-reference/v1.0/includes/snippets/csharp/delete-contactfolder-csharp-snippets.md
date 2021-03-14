---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be519c4b2a0311c4057cfb8a6fc257164db1f651
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.ContactFolders["{contactFolder-id}"]
    .Request()
    .DeleteAsync();

```