---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 661cdee88ec7b1016abae2e0975b1ce67ab10838
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707467"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = await graphClient.Me.ContactFolders["{id}"]
    .Request()
    .GetAsync();

```