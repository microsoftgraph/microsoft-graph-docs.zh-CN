---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2346c4fac2366c19a15b07e733499a5810106ec1f92995b1b692fd7cb05be65f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var room = await graphClient.Places
    .Request()
    .GetAsync();

```