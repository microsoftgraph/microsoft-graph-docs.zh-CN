---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 35dc3d56a2e44a371657d36d373bb486ce3b30d1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736432"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Groups["{groupId}"].Drive
    .Request()
    .GetAsync();

```