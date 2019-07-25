---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 26feeaf30c2e8299f93fb5a7aa9d3f8584be0cbf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892425"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```