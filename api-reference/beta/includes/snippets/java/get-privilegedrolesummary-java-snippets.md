---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 801235ef721e6c3b7ee387f79e9c680c7825d0f4c09e0afaa722fc3eafd0b285
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104362"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleSummary privilegedRoleSummary = graphClient.privilegedRoles("{id}").summary()
    .buildRequest()
    .get();

```