---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 799852a1b08cd00a9ae85c554670fdb4a5ef2cbc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["{educationUser-id}"]
    .Request()
    .GetAsync();

```