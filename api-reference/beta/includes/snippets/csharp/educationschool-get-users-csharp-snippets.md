---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b142b11183f5f3a9a1148c2416e6d8583b939aa1e531a08df2cb660654be8e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Education.Schools["{educationSchool-id}"].Users
    .Request()
    .GetAsync();

```