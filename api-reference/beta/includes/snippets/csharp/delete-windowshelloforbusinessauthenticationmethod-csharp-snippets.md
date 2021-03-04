---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e18b4ccf383ecf80d809ea6790c454828af6466f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433417"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["kim@contoso.com"].Authentication.WindowsHelloForBusinessMethods["_jpuR-TGZtk6aQCLF3BQjA2"]
    .Request()
    .DeleteAsync();

```