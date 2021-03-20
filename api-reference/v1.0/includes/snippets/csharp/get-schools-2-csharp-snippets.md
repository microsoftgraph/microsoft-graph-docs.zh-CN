---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce20d5cc438da5a1ff9db02cb94e801dca857544
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953703"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Schools
    .Request()
    .GetAsync();

```