---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8498a737e32e70b7102c507c9f675eca42248938810c0d18cc5aec124ccd42e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216019"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = new OutlookTaskGroup
{
    Name = "Personal Tasks"
};

await graphClient.Me.Outlook.TaskGroups["{outlookTaskGroup-id}"]
    .Request()
    .UpdateAsync(outlookTaskGroup);

```