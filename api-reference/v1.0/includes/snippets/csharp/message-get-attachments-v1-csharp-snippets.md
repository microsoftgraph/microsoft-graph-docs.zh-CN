---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0eda06646ab6e13fae87ba85cbc3ade043214f4a12879cab38786a2ab550dd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .GetAsync();

```