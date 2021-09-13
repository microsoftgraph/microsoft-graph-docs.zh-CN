---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 314b0134ec5411aec4b4aba3ef2732b54641b6f89b7f8d7885c4a85156dc5f5e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903000"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members
    .Request()
    .GetAsync();

```