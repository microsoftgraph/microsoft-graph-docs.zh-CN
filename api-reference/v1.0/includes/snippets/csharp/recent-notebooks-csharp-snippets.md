---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4551b214f5f71990b57f22950945ea946c89a42caa03d89145a9bda227b39795
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getRecentNotebooks = await graphClient.Me.Onenote.Notebooks
    .GetRecentNotebooks(true)
    .Request()
    .GetAsync();

```