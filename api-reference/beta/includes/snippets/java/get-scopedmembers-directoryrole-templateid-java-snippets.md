---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd04efc2fb77e21628508d4f884d66d80e13c5d3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207718"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedMembers = graphClient.directoryRoles("roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c").scopedMembers()
    .buildRequest()
    .get();

```