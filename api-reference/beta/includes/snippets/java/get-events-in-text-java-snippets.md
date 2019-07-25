---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d74712b2696fb5397c42f5bd2216d8e16c2c18b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867306"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

IEventCollectionPage events = graphClient.me().events()
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview")
    .get();

```