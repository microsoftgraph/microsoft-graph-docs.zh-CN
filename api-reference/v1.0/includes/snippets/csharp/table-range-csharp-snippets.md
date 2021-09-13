---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9988f78b7573026c3ead6ea5fd7f2c78377447a5c45550b7ab498736a0249fd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .Range()
    .Request()
    .GetAsync();

```