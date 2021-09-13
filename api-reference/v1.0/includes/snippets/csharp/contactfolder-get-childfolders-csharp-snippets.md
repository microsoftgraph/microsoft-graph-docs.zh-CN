---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab2fe34994e29fd66d4be932d542e5e15bc772b9864178ce806430f317c8c503
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.ContactFolders["{contactFolder-id}"].ChildFolders
    .Request()
    .GetAsync();

```