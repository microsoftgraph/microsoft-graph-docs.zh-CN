---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6648fb35c3569da0f59c52adcbef28efa1bdd7a2c63428a32580998c5d5f9f31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104862"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{connectedOrganizationId}").internalSponsors("{id}").reference()
    .buildRequest()
    .delete();

```