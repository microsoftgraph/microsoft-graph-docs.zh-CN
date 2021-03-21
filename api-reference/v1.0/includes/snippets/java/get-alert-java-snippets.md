---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 362b5d7151aa985c24c0f7fd4b5c61b53d5a41a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971872"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Alert alert = graphClient.security().alerts("{alert_id}")
    .buildRequest()
    .get();

```