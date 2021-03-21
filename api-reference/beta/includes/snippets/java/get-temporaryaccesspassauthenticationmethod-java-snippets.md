---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcb929c6175df4a9a555a2903530c38409402988
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982463"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethod temporaryAccessPassAuthenticationMethod = graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods("30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30")
    .buildRequest()
    .get();

```