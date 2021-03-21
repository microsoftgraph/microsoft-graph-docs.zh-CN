---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa3fb1f77c01bceaf7589663349c0d680d5a3eb4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967488"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleSettings privilegedRoleSettings = graphClient.privilegedRoles("{id}").settings()
    .buildRequest()
    .get();

```