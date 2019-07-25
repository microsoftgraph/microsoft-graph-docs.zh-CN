---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e786920c0d47d583d1b7d66de97a9a0bfe89c76b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865787"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = graphClient.bookingBusinesses("Fabrikam@M365B489948.onmicrosoft.com")
    .buildRequest()
    .get();

```