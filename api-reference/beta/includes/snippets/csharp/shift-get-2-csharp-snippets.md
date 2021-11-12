---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acb43e593dc362524c9642c59332a6e6694598dd6afe5aea3c6a15cc7afdd7e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shiftPreferences = await graphClient.Users["{user-id}"].Settings.ShiftPreferences
    .Request()
    .GetAsync();

```