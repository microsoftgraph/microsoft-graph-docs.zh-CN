---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a093e1286136e2b1844ed7f3ce3c6769fa7fa0110c98e1c03d480b389ac031c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409607"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnits = await graphClient.Directory.AdministrativeUnits
    .Request()
    .GetAsync();

```