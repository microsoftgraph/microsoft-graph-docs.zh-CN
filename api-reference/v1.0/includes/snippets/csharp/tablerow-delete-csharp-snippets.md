---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49112f323c83451f8c87d51e7aeb93b12d9bbb614c701b7ccdd85fe0c05fcafc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows["{workbookTableRow-id}"]
    .Request()
    .DeleteAsync();

```