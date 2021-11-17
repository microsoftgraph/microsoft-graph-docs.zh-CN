---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b91d76f9dcd3f360121989ca3ad40980e5b84b6a1e97e9ec716bc9cd1cd393a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278056"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRule = await graphClient.Me.MailFolders["{mailFolder-id}"].MessageRules["{messageRule-id}"]
    .Request()
    .GetAsync();

```