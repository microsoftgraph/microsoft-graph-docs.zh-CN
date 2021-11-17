---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5950bda90ecb628aa8a3af268f295147f8c3c5d760de979fda88e948f0e88e58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105814"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var businessFlowTemplates = await graphClient.BusinessFlowTemplates
    .Request()
    .GetAsync();

```