---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 016c6af89900d165277a5b182c7c32042eef3e1b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856453"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.MailFolders["{id}"].Messages
    .Request()
    .GetAsync();

```