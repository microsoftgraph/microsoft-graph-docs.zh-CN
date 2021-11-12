---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 167ea8cbdd15d3a8937f8184eacac9f073695b9394c5fbc147a608b7ac0d7963
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["{message-id}"]
    .Request()
    .Expand("mentions")
    .GetAsync();

```