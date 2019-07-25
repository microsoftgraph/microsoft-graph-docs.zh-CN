---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0bda72b6085f3291c6fa3f3b639bc3a74328141f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865402"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IBookingCurrencyCollectionPage bookingCurrencies = graphClient.bookingCurrencies()
    .buildRequest()
    .get();

```