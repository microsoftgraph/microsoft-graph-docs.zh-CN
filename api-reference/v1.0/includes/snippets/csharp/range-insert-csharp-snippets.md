---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07d607f27e2cd5bd7a74f4bc0b813bdde73793aec6ba78b9d4f1ccc5d36a70ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162543"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = "shift-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Insert(shift)
    .Request()
    .PostAsync();

```