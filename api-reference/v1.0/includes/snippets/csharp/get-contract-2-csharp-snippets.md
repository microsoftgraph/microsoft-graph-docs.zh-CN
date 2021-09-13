---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2a3beeeb64ee044991a0faf1e201ecbd109cc2615dcccee00a9c81731ba786d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contracts = await graphClient.Contracts
    .Request()
    .GetAsync();

```