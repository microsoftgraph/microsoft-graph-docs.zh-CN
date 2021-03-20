---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd8415bf9e8be5c0deca4f1d1775e70a2fedc9dc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953300"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fido2Methods = await graphClient.Me.Authentication.Fido2Methods
    .Request()
    .GetAsync();

```