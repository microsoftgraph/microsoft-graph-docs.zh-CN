---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2f1e19042fe6d8a2eaa8659bf04f5f88cd62be70
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comments = await graphClient.Drive.Root.Workbook.Comments
    .Request()
    .GetAsync();

```