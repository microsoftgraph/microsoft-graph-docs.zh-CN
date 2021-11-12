---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f68ef12f15d1f894a318b6ad355bb3d1464afa78634c51957f6cb83e37853053
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReasons = await graphClient.Teams["{team-id}"].Schedule.TimeOffReasons
    .Request()
    .GetAsync();

```