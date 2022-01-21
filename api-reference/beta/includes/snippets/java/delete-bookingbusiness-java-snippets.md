---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27ae8f9864d346c44b93c9e3cd920ea5db47e8c7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130144"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("fabrikam@contoso.onmicrosoft.com")
    .buildRequest()
    .delete();

```