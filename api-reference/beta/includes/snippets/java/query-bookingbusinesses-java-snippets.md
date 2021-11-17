---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82e590f93fb8882d44b40a47b64958c4a59e816f1f3b73799c53f4a6413eede3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903150"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("query", "Adventure"));

BookingBusinessCollectionPage bookingBusinesses = graphClient.bookingBusinesses()
    .buildRequest( requestOptions )
    .get();

```