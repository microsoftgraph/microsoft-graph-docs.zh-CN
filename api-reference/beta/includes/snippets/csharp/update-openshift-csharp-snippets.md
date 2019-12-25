---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 124feffaa45acece50e0d4ef64f7cee6fc43902e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShifts = new OpenShift
{
    SharedOpenShift = new OpenShiftItem
    {
        OpenSlotCount = 99
    },
    DraftOpenShift = new OpenShiftItem
    {
        OpenSlotCount = 99
    },
    SchedulingGroupId = "TAG_f914d037-00a3-4ba4-b712-ef178cbea263"
};

await graphClient.Teams["{id}"].Schedule.OpenShifts
    .Request()
    .UpdateAsync(openShifts);

```