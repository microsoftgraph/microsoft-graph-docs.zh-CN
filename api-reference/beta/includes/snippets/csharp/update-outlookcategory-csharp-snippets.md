---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0216fe8a6d53a47644219c0efb2292f72db7ae38
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = new OutlookCategory
{
    Color = CategoryColor.Preset15
};

await graphClient.Me.Outlook.MasterCategories["{outlookCategory-id}"]
    .Request()
    .UpdateAsync(outlookCategory);

```