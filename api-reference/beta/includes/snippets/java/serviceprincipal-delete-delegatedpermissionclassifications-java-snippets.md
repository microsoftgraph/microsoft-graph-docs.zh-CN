---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48078ba50272267526f5ee6ffa0bf0ae6223460a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976233"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").delegatedPermissionClassifications("{id}")
    .buildRequest()
    .delete();

```