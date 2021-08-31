---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c13565a1a57c610c389bbcefe6bb8a1f1dae55d836dba68c8ec247e621b1c07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Drive.Items["{driveItem-id}"].Content
    .Request()
    .GetAsync();

```