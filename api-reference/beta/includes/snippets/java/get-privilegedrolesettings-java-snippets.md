---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ce284a11525a9f566e5383fdaa2f67b28b3674ff3baacad0051aa83707ae221
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleSettings privilegedRoleSettings = graphClient.privilegedRoles("{id}").settings()
    .buildRequest()
    .get();

```