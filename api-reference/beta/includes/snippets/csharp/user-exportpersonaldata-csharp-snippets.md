---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 991fc7fdb44c0af9bd4567da5e09e55983deb958
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var storageLocation = "storageLocation-value";

await graphClient.Users["{id}"]
    .ExportPersonalData(storageLocation)
    .Request()
    .PostAsync();

```