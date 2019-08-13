---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 608a65599ed905c4e36466db4f1ab2c223b50c73
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetEmailActivityUserDetail("D7")
    .Request()
    .GetAsync();

```