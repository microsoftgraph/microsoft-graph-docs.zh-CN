---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e62a3b202b4f0fa4896fa48c687ee0e0c96ed891a4baa1adea9d42960efb9db5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221064"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Drive.Root.Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range()
    .ColumnsBefore(2)
    .Request()
    .GetAsync();

```