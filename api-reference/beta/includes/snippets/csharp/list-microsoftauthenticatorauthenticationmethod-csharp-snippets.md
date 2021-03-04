---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cfb7fc32d1760a43ddd6d7159b8333f306648ca
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447950"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoftAuthenticatorMethods = await graphClient.Users["anirban@contoso.com"].Authentication.MicrosoftAuthenticatorMethods
    .Request()
    .GetAsync();

```