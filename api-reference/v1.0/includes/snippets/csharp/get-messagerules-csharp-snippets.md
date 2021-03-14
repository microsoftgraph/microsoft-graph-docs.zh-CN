---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e81c66098cd4d1dc7835c0dac05bd9f5885f42a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRules = await graphClient.Me.MailFolders["{mailFolder-id}"].MessageRules
    .Request()
    .GetAsync();

```