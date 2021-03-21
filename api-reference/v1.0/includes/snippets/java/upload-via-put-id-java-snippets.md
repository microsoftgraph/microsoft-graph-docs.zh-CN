---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c344ceffbf8889c411dcdda035ac2f7c1e1173a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] stream = Base64.getDecoder().decode("The contents of the file goes here.");
    graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .put(stream);

```