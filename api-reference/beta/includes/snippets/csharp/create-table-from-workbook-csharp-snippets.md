---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 790d5a3282295635bd256742e585aaf5a9cd60f91c02402b372e9f6142ca158a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "A1:D8";

var hasHeaders = false;

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables
    .Add(hasHeaders,address)
    .Request()
    .PostAsync();

```