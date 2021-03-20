---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d1630c707b063683f2e1f6a593c2dfebbe63794
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969457"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}")
    .buildRequest()
    .delete();

```