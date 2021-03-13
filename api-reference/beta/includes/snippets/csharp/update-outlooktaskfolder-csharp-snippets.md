---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e4b0d289a39d7f831c1a78a659478b4506d1703
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = new OutlookTaskFolder
{
    Name = "Charity work"
};

await graphClient.Me.Outlook.TaskFolders["{outlookTaskFolder-id}"]
    .Request()
    .UpdateAsync(outlookTaskFolder);

```