---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 843622052b619fb936eb28e927e278b1810f3885e9b9f30a3ed634b8dbf585f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164235"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comments = await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments
    .Request()
    .GetAsync();

```