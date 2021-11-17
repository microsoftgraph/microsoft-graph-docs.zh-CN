---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 247eb3e1dfd55aab46482620bf68be2550bbcf1b2386388b564c02641126b3ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phoneMethods = await graphClient.Me.Authentication.PhoneMethods
    .Request()
    .GetAsync();

```