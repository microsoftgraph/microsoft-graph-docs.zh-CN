---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21fcca947cd0121abe3b1fe4ed7e88480a92c8ab5d1f70caa146fd617cb6014c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161536"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var history = await graphClient.RiskyUsers["{riskyUser-id}"].History
    .Request()
    .GetAsync();

```