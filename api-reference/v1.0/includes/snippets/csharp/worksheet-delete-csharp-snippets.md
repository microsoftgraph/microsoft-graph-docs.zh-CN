---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dae17b78c6e7395c6bc7ef9790d0e516c9bf99c22194dec89a40e9bda4e36c74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Request()
    .DeleteAsync();

```