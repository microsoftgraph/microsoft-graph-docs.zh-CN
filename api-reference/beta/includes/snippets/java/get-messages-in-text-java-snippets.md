---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7436434d469f7323cb31c72a04b2ee2467ca0a18
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

MessageCollectionPage messages = graphClient.me().messages()
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,uniqueBody")
    .get();

```