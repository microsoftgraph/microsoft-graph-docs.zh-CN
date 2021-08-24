---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1175fa8a47638c96794676f5bd29d96833ef4a704e8ee69b7ca519b119516cf5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Groups
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select("displayName,description,mailNickname")
    .GetAsync();

```