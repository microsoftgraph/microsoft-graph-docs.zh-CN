---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b249a70008abbcd2f0caa581afdd29bb99e0367c3f2fa64376f47895e2241fcc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163595"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Me
    .Request()
    .GetAsync();

```