---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e83b9e95e87c699afd7fbbe54418078263f7728
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619176"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = await graphClient.Education.Classes["11023"]
    .Request()
    .GetAsync();

```