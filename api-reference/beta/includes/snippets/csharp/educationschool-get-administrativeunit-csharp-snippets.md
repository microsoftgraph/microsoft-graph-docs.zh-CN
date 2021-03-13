---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56c4bb9f4b86098a2bedd16ca6bd7303c67e1db2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.Education.Schools["{educationSchool-id}"].AdministrativeUnit
    .Request()
    .GetAsync();

```