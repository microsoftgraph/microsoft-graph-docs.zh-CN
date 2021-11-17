---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc70603228dd6360eb5d1e21ac27e11aaebf6cfe9c05895e8184c0be3417a023
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105527"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var controls = await graphClient.Programs["{program-id}"].Controls
    .Request()
    .GetAsync();

```