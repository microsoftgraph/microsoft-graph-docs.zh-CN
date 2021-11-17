---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc86ed84ddf3c3a6500f1083939b9c022ea58a728460d301ac191a1da0d1fdbb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Request()
    .DeleteAsync();

```