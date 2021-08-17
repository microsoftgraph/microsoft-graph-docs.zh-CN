---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 362a30a64663251b92e39bb1f1080944cbc5afdda05d7d7e5d8288f676d00a46
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Groups["{group-id}"].TransitiveMembers
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:tier")
    .Select("displayName,id")
    .OrderBy("displayName")
    .GetAsync();

```