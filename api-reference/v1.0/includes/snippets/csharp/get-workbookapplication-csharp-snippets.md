---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f12716d590a74acd1ba19cf02dc57175a4313b98c5b03e3005460884b66e8e62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookApplication = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Application
    .Request()
    .GetAsync();

```