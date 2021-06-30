---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21362ae1983f7022201f975d59c0d50f52f373ed
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207696"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedMembers = graphClient.directoryRoles("41d12a2f-caa8-4e3e-ba14-05e5102ce085").scopedMembers()
    .buildRequest()
    .get();

```