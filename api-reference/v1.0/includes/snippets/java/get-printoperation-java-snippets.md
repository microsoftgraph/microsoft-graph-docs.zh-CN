---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0696aa5a383690212727c14242957d74c74ef489
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintOperation printOperation = graphClient.print().operations("{printOperationId}")
    .buildRequest()
    .get();

```