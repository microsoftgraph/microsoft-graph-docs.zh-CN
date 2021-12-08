---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c521a66b8d6ec5a26fc44519b5c24a48fa33fe7a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340691"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectedOrganization connectedOrganization = graphClient.identityGovernance().entitlementManagement().connectedOrganizations("04e7fa5f-fa5f-04e7-5ffa-e7045ffae704")
    .buildRequest()
    .get();

```