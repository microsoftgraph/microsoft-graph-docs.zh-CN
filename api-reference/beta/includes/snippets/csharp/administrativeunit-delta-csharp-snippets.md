---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb4a3429fc694b229daa807646ae32c3ade85acd15159c94ff2bbd01872b9d9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.AdministrativeUnits
    .Delta()
    .Request()
    .GetAsync();

```