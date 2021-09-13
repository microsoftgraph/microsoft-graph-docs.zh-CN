---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32ee75758ad2fceba5450ddf69d879e06baa1a51891de9b0c71808b9ed2b3d83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277512"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var linkedResource = new LinkedResource
{
    WebUrl = "http://microsoft.com",
    ApplicationName = "Microsoft",
    DisplayName = "Microsoft"
};

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"].LinkedResources["{linkedResource-id}"]
    .Request()
    .UpdateAsync(linkedResource);

```