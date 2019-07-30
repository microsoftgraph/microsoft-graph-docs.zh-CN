---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 806c72db5d80cb7fb24e6cd2d668ef125c946b3d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933808"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"].Unfollow
    .Request()
    .DeleteAsync();

```