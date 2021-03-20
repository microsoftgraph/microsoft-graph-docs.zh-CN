---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 826637c3f1d83ad7a820273cd97e13a02ee10c05
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945758"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var names = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names
    .Request()
    .GetAsync();

```