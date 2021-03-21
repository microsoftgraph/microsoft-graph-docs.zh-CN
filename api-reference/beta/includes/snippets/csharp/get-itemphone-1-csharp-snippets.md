---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fcb75e05c0e4d5e29cef79a625b3fcc559f71ec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954538"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPhone = await graphClient.Me.Profile.Phones["{itemPhone-id}"]
    .Request()
    .GetAsync();

```