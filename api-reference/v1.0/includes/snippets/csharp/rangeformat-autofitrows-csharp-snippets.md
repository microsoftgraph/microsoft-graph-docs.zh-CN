---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4609692f06a83db9a92dfd40a002586b0367afa61f7a6ac9856a66d2209dd14b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format
    .AutofitRows()
    .Request()
    .PostAsync();

```