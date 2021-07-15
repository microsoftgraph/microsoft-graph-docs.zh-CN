---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24741c43a9bb8682c067a42f24722763de9fa5c5
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441389"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUser riskyUser = graphClient.tenantRelationships().managedTenants().riskyUsers("{riskyUserId}")
    .buildRequest()
    .get();

```