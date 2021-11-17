---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8cba7a71db00c6a59e5224413ac93421b7771ce55e53a6fd054520dc383dad3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161671"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = await graphClient.Me.Profile.Anniversaries["{personAnnualEvent-id}"]
    .Request()
    .GetAsync();

```