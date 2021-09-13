---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f81f33c0cd2e5c248c390b302cbffbe016b8a2e315f8d398854beccd303421b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = await graphClient.GroupSettings["{groupSetting-id}"]
    .Request()
    .GetAsync();

```