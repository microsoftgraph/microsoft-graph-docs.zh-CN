---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e4b05b62b8b4d17a335ecf3c7823c804a3cc1cf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffRequests = await graphClient.Teams["{id}"].Schedule.TimeOffRequests
    .Request()
    .GetAsync();

```