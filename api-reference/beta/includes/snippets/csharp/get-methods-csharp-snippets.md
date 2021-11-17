---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 490591f96a07df8fd9e490e60c769b1b37f46bbcd42250131d1c14f7e15a99de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var methods = await graphClient.Me.Authentication.Methods
    .Request()
    .GetAsync();

```