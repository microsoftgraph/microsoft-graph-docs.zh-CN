---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b36f64ec441de78f9dc17e0a26137231abe602eebf45af8da7179639d5cd003
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221193"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Calendar.Events
    .Request()
    .GetAsync();

```