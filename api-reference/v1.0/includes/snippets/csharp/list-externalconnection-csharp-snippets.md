---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d28a002522d7402c029ed1fcfb59eed661cded76c4ea251e2fedbf86e642f17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332600"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connections = await graphClient.Connections
    .Request()
    .GetAsync();

```