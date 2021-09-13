---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df1e6edfb0f5d1d8c9a77f965282459916479abd540f2124dc1c6865b5dc974d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Sort
    .Clear()
    .Request()
    .PostAsync();

```