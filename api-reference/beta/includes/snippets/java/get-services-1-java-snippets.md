---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0247f0b10fa614ea002347b23a2d1f1d42f3c6d0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130046"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingServiceCollectionPage services = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").services()
    .buildRequest()
    .get();

```