---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdba49fb6f228422a70ddf4708d59742786c57dd
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2020
ms.locfileid: "46657970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Reports
    .GetM365AppUserCounts("D7").Content
    .Request()
    .GetAsync();

```