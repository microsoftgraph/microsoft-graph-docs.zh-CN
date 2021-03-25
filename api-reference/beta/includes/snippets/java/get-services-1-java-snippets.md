---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6e8593204459f8a22c6289729e93e80052a802b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210856"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingServiceCollectionPage services = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").services()
    .buildRequest()
    .get();

```