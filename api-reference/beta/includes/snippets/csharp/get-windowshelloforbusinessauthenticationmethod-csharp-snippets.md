---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70e4fe434f375768e202f436e3022d6bbdf75efbb809eaea6e729d3a514bd75b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsHelloForBusinessAuthenticationMethod = await graphClient.Users["{user-id}"].Authentication.WindowsHelloForBusinessMethods["{windowsHelloForBusinessAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```