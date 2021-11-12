---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95c179dfb4e36ed00217937e459118b96ea9b4b17ed4ac5826865cd7b0dc690f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218815"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("A1:Z10")
    .VisibleView()
    .Range()
    .Request()
    .GetAsync();

```