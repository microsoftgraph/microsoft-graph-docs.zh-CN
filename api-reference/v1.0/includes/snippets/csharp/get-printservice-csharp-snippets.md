---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1816ea2583dd41542354e581eebe4bd8e15b2a1f41cf6ab073e0ffce304d1aae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904065"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printService = await graphClient.Print.Services["{printService-id}"]
    .Request()
    .GetAsync();

```