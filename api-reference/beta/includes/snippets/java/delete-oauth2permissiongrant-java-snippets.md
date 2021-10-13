---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2e865ac8480c75acc1d1824700c964b8b0d3b5b7cbecbcf28670cf0ef86e5ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277768"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.oauth2PermissionGrants("{id}")
    .buildRequest()
    .delete();

```