---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 822716da6b5bb47471a92b6d31703d9e25a5f500
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873891"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$orderby", "LastUsed/LastAccessedDateTime desc"));

IUsedInsightCollectionPage used = graphClient.me().insights().used()
    .buildRequest( requestOptions )
    .get();

```