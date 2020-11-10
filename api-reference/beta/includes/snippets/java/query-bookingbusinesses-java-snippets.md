---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31d6ee6995c11a2ece8cc1e0311a78552d631ea3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960768"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("query", "Adventure"));

IBookingBusinessCollectionPage bookingBusinesses = graphClient.bookingBusinesses()
    .buildRequest( requestOptions )
    .get();

```