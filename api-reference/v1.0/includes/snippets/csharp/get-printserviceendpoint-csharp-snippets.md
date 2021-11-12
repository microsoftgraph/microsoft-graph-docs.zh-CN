---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b3a0449023b073481c2f1edbe3993cdba401565fa9e92789c78867a8ecab250
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printServiceEndpoint = await graphClient.Print.Services["{printService-id}"].Endpoints["{printServiceEndpoint-id}"]
    .Request()
    .GetAsync();

```