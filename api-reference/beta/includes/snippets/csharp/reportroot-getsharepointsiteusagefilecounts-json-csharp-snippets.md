---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9ebd00539711b8efc101ec2024a492ccef5b028d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359551"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageFileCounts = await graphClient.Reports
    .GetSharePointSiteUsageFileCounts("D7")
    .Request()
    .GetAsync();

```