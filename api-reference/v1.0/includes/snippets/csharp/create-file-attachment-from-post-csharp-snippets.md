---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2d3bb8ba05dab7d20f4d9d55e4ee7f168a1688b1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467533"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    Name = "name-value",
    ContentBytes = "base64-contentBytes-value"
};

await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```