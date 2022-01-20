---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5f8c3d54feb479930ae15965e3b75b9f710be4a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094734"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomerCollectionPage customers = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").customers()
    .buildRequest()
    .get();

```