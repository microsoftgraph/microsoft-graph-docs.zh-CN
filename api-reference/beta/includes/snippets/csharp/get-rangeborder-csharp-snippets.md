---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd011014e215592a995a758adcca76b6d6176c3b762d59687404bfdf0ae29585
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeBorder = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Borders["{workbookRangeBorder-id}"]
    .Request()
    .GetAsync();

```