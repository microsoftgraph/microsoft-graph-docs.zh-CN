---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f242019001f6b5d7b226a99c39c7f1510f3f06b7c5cebd93687c31353c934ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218773"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

Message message = graphClient.me().messages("AAMkAGI1AAAoZCfHAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,uniqueBody")
    .get();

```