---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9095f2d2b7439d99c9c4d7834bd5416846a7e69f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613573"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teachers = await graphClient.Education.Classes["11023"].Teachers
    .Request()
    .GetAsync();

```