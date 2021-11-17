---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26bb783ffb11d62c021076d19e26f5b7bd4b2e29eb5f1fb20a11ecdfb8c50ce7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassMethods = await graphClient.Me.Authentication.TemporaryAccessPassMethods
    .Request()
    .GetAsync();

```