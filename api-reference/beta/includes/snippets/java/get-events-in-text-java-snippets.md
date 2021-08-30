---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f50a8007f25c985d4475a7d3ba9921457d458de05c70c5ba96d3b9d235d488f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164060"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

EventCollectionPage events = graphClient.me().events()
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview")
    .get();

```