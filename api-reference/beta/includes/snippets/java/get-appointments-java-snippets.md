---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 472c2473e9f09a93b5e703e010c7528492e64069
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865745"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IBookingAppointmentCollectionPage appointments = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments()
    .buildRequest()
    .get();

```