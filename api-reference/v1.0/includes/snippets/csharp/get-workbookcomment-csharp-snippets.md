---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4c36e15fabd9af3f49938d743dcac251299aee73ace8903e7f95a4046f34914
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903197"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookComment = await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments["{workbookComment-id}"]
    .Request()
    .GetAsync();

```