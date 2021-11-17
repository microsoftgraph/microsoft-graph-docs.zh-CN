---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7580337804e0887d3de8d2db7f24574926a353b9c0b3f1abfb93fd075d338ae4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279484"
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