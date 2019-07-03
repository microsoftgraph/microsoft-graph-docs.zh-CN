---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0f574ddf0abdca1d6271ffb10abaff74e56a42a2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520526"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityStorage = await graphClient.Reports.GetOffice365GroupsActivityStorage('D7')
    .Request()
    .GetAsync();

```