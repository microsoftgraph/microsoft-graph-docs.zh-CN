---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64e3eda9e9f75d4ccd2f5770d828837f2493076a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Drives["{driveId}"]
    .Request()
    .GetAsync();

```