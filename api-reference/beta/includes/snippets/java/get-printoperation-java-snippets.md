---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01eb54fe15b36247e9656d9cca1de34e479dcb98
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983082"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintOperation printOperation = graphClient.print().operations("{id}")
    .buildRequest()
    .get();

```