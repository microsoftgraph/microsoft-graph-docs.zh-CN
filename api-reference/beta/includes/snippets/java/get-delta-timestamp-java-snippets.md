---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e150a0fb59ee2617968096448e1f867772c5e21f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019926"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("token", "2021-09-29T20:00:00Z"));

DriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta()
    .buildRequest( requestOptions )
    .get();

```