---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e2ecec4f233cb5480e012685211c16b7e6fef2227a51a20db7d07185fb0829c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowAttributes = await graphClient.Identity.UserFlowAttributes
    .Request()
    .GetAsync();

```