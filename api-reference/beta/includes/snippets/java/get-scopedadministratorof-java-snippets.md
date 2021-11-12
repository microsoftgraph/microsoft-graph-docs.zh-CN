---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b6b45ecaf2c9a054fb5e71644853bc6f1826c975fc5ddaa5309d3f7f40427ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333615"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedRoleMemberOf = graphClient.me().scopedRoleMemberOf()
    .buildRequest()
    .get();

```