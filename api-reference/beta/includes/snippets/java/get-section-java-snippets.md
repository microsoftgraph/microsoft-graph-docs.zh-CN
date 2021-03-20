---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 848b6db7b72a052e1af2454c210464b302b9ae4e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974669"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = graphClient.me().onenote().sections("{id}")
    .buildRequest()
    .get();

```