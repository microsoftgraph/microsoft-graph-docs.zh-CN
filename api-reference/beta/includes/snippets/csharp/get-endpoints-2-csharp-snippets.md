---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50fb9b3d16dc051faae8ce44b0ffdd1225cae5d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961478"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoints = await graphClient.Print.Services["{printService-id}"].Endpoints
    .Request()
    .GetAsync();

```