---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a4a3a4dce1d627fbfebaf2003664bd2073b4299bed49690c21d16d0eb4280e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .RemoveFavorite()
    .Request()
    .PostAsync();

```