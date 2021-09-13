---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 297ca04bc86cc89709e92d5bd597eef9e873fc2afde0deb8c05363f5f373353f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithMe = await graphClient.Me.Drive
    .SharedWithMe()
    .Request()
    .GetAsync();

```