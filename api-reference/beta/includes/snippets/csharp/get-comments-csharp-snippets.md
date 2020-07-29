---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb6cd536319bc63c9376e22f84e6ba06dd7e71db
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comments = await graphClient.Drive.Items["{id}"].Workbook.Comments
    .Request()
    .GetAsync();

```