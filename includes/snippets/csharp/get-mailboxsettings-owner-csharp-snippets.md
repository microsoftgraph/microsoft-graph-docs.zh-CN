---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 307fe725d2cfa53d80f1c92d486b37cbbdd7d583cbcaf7d146a95798b6f521dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users["AlexW@contoso.OnMicrosoft.com"]
    .Request()
    .Select("MailboxSettings")
    .GetAsync();

var mailboxSettings = users.MailboxSettings;

```