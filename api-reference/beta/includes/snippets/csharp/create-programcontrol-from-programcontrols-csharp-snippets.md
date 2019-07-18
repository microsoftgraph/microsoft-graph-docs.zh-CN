---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5d9ad6727ad4bb483bf9937cc660225521efd67d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControl = new ProgramControl
{
    ControlId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    ControlTypeId = "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    ProgramId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
};

await graphClient.ProgramControls
    .Request()
    .AddAsync(programControl);

```