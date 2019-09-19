---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e82accc561d61fa874d5eb47c41cfa63d5850cf
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041944"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

Message message = graphClient.me().messages("AAMkAGI1AAAoZCfHAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,uniqueBody")
    .get();

```