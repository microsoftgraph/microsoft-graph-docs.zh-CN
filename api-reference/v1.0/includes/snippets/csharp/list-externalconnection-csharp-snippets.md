---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1151894523cbf9169a00f0618cf36b3859eb17cd
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connections = await graphClient.External.Connections
    .Request()
    .GetAsync();

```