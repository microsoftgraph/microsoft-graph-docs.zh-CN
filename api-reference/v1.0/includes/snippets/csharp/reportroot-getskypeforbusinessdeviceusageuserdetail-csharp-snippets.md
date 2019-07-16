---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2b470a435da2180dad2a3509ea091b78ecd7bba2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738254"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessDeviceUsageUserDetail('D7')
    .Request()
    .GetAsync();

```