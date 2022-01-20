---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c404581826e2fa342f9a34710bf6c04a05d5506
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106852"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").customers("80b5ddda-1e3b-4c9d-abe2-d606cc075e2e")
    .buildRequest()
    .delete();

```