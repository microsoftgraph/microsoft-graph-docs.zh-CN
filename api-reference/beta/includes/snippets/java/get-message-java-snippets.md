---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7297a81e2ea0cc7384799f8755afbfbd92085847298e9b11c410321a65c52253
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279069"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkAGI1AAAoZCfHAAA=")
    .buildRequest()
    .get();

```