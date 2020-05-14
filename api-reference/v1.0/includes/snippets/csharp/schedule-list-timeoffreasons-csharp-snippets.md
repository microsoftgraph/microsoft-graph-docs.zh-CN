---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cedf084e58b562c9cf8574106ac837853aad260
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44218459"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReasons = await graphClient.Teams["{teamId}"].Schedule.TimeOffReasons
    .Request()
    .GetAsync();

```