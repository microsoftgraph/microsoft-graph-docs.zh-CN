---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 399ae9a404286b1540d18d31008ef61a4c7a59be
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deployments = await graphClient.Admin.Windows.Updates.Deployments
    .Request()
    .GetAsync();

```