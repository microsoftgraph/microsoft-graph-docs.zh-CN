---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d708df402efdb177847d2af94de4f4a5c6b3ff9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778319"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.MailFolders["{mailFolder-id}"].Messages
    .Request()
    .GetAsync();

```