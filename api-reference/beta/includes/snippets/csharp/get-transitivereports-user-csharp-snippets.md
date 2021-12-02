---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a88262e1c9b70c11d2c61f79a5e1c94cabc9728389e1fa842a42be6181decdf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277933"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Users["{user-id}"].TransitiveReports.$count
    .Request()
    .GetAsync();

```