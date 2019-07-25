---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 68db4a30fc67c100faf93fdc5d6619f1575e1991
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729054"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = await graphClient.Me.Outlook.MasterCategories["de912e4d-c790-4da9-949c-ccd933aaa0f7"]
    .Request()
    .GetAsync();

```