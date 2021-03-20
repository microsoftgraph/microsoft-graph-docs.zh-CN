---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 189aabf7420f5dbc5c03fcffbc5e69bb78fc6001
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941699"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Me.Classes
    .Request()
    .GetAsync();

```