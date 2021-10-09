---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46a6e2d0de066c83790595396380d075ad8f39be2ec3272965cc00b75ceceb9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "84b80893-8749-40a3-97b7-68513b600544",
    "5d6059b6-368d-45f8-91e1-8e07d485f1d0"
};

var types = new List<String>()
{
    "user"
};

await graphClient.DirectoryObjects
    .GetByIds(ids,types)
    .Request()
    .PostAsync();

```