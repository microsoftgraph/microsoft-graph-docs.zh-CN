---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed1bcdc43e8ecde7e7da7098e7ded09a020fd345
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334847"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IServicePrincipalCollectionPage serviceprincipals = graphClient.serviceprincipals()
    .buildRequest()
    .get();

```