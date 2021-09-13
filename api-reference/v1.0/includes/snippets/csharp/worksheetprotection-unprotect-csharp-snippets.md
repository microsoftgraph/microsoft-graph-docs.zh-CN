---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07c457fc341bbb52c4e33a4d61c36650629f0ae3ede13595829b7f40031ae3e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Protection
    .Unprotect()
    .Request()
    .PostAsync();

```