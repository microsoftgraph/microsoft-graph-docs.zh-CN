---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6356667ba2064bde41812626bb04ac717ae24aef696dc68ec582a2cd1e143ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902379"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.PrinterShares["{printerShare-id}"].AllowedUsers["{user-id}"].Reference
    .Request()
    .DeleteAsync();

```