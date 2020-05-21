---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 573fea081db1cb490ae85f78d00f4920eb41e111
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"]
    .Archive(null)
    .Request()
    .PostAsync();

```