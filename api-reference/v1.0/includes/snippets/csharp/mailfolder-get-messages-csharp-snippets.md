---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b8b98d40a269a3a2ba1143fec231275ff2c1a6cc2567271d37db04f456a606f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904131"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.MailFolders["{mailFolder-id}"].Messages
    .Request()
    .GetAsync();

```