---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b15847b6dcc953e17203a936b4eb90277e239406
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137692"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com")
    .unpublish()
    .buildRequest()
    .post();

```