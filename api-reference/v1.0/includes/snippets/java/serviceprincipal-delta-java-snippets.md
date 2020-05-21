---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07d0ff96d711efaa8a7163012b84ffd915fd2bff
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334112"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = graphClient.servicePrincipals("delta")
    .buildRequest()
    .get();

```