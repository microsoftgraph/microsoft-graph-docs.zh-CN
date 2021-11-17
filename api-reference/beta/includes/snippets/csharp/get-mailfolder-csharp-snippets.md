---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25421fb01d34a064fdedf26216399a3dd61d9260da677d328a923263836b313c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279060"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Request()
    .GetAsync();

```