---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 496af323e2b8b91c06be6f130185236b082920bb
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335155"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$orderby", "LastUsed/LastAccessedDateTime"));

IUsedInsightCollectionPage used = graphClient.me().insights().used()
    .buildRequest( requestOptions )
    .get();

```