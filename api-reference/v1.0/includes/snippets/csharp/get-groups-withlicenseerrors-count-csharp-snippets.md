---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c6b3503f9e16f99f1c02b30ecebd5c2db6d99a9
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("hasMembersWithLicenseErrors+eq+true,")
    .Select("id,displayName")
    .GetAsync();

```