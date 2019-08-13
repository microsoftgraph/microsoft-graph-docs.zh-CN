---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f78b9950402aa3e1b31bfa29fb66e0dccbc4e5e9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358585"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserDetail = await graphClient.Reports
    .GetYammerActivityUserDetail("D7")
    .Request()
    .GetAsync();

```