---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6719535c2d7caa37aad26e982ccb7168bf9a0c5a1245e83944a0fd17a4ed733
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = new OutlookTaskGroup
{
    Name = "Leisure tasks"
};

await graphClient.Me.Outlook.TaskGroups
    .Request()
    .AddAsync(outlookTaskGroup);

```