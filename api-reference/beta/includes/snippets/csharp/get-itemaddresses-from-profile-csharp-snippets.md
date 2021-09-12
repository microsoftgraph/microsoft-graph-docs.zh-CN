---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a4d9175134e0741293979ba4abfda679789e7723786daf483778c6b7435b493
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218998"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addresses = await graphClient.Me.Profile.Addresses
    .Request()
    .GetAsync();

```