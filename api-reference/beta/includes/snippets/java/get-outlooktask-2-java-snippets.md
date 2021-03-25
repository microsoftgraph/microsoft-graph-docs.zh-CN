---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aa583a7f8ea77217db1ba7d3dbb1d63315acc55
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208634"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

OutlookTask outlookTask = graphClient.me().outlook().tasks("AAMkADA1MHgwAAA=")
    .buildRequest( requestOptions )
    .get();

```