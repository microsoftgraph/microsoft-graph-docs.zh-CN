---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33b4f3874365b4a33d9b0b3d269642c01aacbe1d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442317"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.PrinterShares["{id}"].AllowedUsers["{id}"].Reference
    .Request()
    .DeleteAsync();

```