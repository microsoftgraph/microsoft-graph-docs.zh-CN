---
description: 自动生成的文件。 不修改
ms.openlocfilehash: be89f9351dc996b01b6b64f05002de8a46cbe33f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865681"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IBookingServiceCollectionPage services = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").services()
    .buildRequest()
    .get();

```