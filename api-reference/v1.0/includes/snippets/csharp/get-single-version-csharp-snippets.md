---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d09e9486281cfa4f5fbdfe9a54bb4e3349522736f6ea224117ab2aab98c3bab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409737"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItemVersion = await graphClient.Me.Drive.Items["{driveItem-id}"].Versions["{driveItemVersion-id}"]
    .Request()
    .GetAsync();

```