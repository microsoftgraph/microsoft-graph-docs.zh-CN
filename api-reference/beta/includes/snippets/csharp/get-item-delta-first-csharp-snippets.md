---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 910faa4724cf2bf1115079bb26fc5ea84c56297edcfb2fe800a563c3ed2a1b0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root
    .Delta()
    .Request()
    .GetAsync();

```