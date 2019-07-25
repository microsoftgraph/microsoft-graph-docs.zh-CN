---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c79ba85648ca154b612ab3d1f380baf8e8e3ee70
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Groups["37df2ff0-0de0-4c33-8aee-75289364aef6"].Threads["AAQkADJizZJpEWwqDHsEpV_KA=="].Posts["AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA="].Extensions["Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"]
    .Request()
    .GetAsync();

```