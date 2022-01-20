---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d545be5f0c0c1713505ff2d97a8a09c736cfb395
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116557"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").appointments("AAMkADKqAAA=")
    .buildRequest()
    .delete();

```