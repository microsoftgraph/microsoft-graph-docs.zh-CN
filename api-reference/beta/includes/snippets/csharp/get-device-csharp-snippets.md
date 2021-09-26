---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acfe86474750fe0847e9e4c579828bfa9e5cc0c14ab6799f54a9e157dc717b1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = await graphClient.Devices["{device-id}"]
    .Request()
    .GetAsync();

```