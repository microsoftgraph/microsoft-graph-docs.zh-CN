---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f68f92a9b9635246ddbb5053587c5244b47f8957326e337215bcbf0ac70732a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedGroups = await graphClient.Print.Shares["{printerShare-id}"].AllowedGroups
    .Request()
    .GetAsync();

```