---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eeb81d7f065b29dc6c6794363ef557a2ba8aa960fa0b453ba296986a13ea7d30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105742"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders["{mailFolder-id}"].Messages
    .Delta()
    .Request()
    .GetAsync();

```