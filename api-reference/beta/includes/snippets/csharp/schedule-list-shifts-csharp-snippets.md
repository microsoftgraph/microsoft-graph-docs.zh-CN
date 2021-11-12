---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0e93c34ed479481e2952c242232eafebba699bfc06ffe439c796428d98b7d1f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161518"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shifts = await graphClient.Teams["{team-id}"].Schedule.Shifts
    .Request()
    .Filter("sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z")
    .GetAsync();

```