---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c25e3ff664b967d064e8cf685ef3381baa3ca4b
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844536"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ApiConnectors["{id}"]
    .Request()
    .DeleteAsync();

```