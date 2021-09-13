---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8307f6577fb42c78f1015733606587f407a83c59ed9d473508a9275399e3e0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219479"
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