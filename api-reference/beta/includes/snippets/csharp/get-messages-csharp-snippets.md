---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4a1ce43601229546197744f7953499584986f06f1201f7fa83ccc2d433abc59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105490"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Select("sender,subject")
    .GetAsync();

```