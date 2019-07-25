---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31d6ee6995c11a2ece8cc1e0311a78552d631ea3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865633"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("query", "Adventure"));

IBookingBusinessCollectionPage bookingBusinesses = graphClient.bookingBusinesses()
    .buildRequest( requestOptions )
    .get();

```