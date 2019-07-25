---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 43f78a43b4be3db290369259f1d0b917cee54c1b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865716"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IBookingCustomerCollectionPage customers = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers()
    .buildRequest()
    .get();

```