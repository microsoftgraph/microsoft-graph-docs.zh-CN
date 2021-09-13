---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c36e92325288dfefff57f886f7666d34e68f0aca4828f2dae04fa988019a9f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessions = await graphClient.Communications.CallRecords["{callRecords.callRecord-id}"].Sessions
    .Request()
    .GetAsync();

```