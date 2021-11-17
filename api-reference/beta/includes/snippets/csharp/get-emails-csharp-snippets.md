---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9b02fa8f058d965dcdf9f9bf6995732d4b73bdd864aea3a8e717aab6b2224dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273848"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emails = await graphClient.Me.Profile.Emails
    .Request()
    .GetAsync();

```