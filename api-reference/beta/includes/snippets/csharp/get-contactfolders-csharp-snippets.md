---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e840ad0911788e8b40da97740a889cdd70a708d40c22010c73f87483d04f0b18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162849"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolders = await graphClient.Me.ContactFolders
    .Request()
    .GetAsync();

```