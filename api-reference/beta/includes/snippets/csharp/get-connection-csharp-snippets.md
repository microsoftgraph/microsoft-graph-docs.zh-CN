---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aedf0d88214b5fa1f69ff85826990c718bf8ca0
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573218"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = await graphClient.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .GetAsync();

```