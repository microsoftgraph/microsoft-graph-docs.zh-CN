---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c57e4c0e303f24f2c2cb3960b560e5ac39c516652d735f8af7ee2a338d32877c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Operations
    .Request()
    .GetAsync();

```