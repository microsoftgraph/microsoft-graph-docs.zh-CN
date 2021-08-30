---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8de761332122e50463994c8d2c07983f273440a5043b249eb4c8b4d257b8150
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104035"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = await graphClient.Applications["{application-id}"]
    .Request()
    .GetAsync();

```