---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df8cb4b935b72d87619c6a874ad9e6a9fcb29df35bfc5f6cda4d95170bd4030f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format
    .AutofitColumns()
    .Request()
    .PostAsync();

```