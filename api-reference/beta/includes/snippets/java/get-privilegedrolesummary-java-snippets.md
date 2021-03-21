---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ad41cbda4ef5a0d227cca7fd7c9a1597f370b73
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968045"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleSummary privilegedRoleSummary = graphClient.privilegedRoles("{id}").summary()
    .buildRequest()
    .get();

```