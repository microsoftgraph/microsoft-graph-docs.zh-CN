---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18576a9a026d9dbff4c09fde918839481db3ebc7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Items["{item-id}"].Children
    .Request()
    .Expand("thumbnails")
    .GetAsync();

```