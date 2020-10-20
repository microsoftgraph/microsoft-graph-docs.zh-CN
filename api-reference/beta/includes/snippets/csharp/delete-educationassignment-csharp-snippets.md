---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e71a139481db163d49297028d84c53788add991
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610271"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11014"].AssignmentCategories["19002"]
    .Request()
    .DeleteAsync();

```