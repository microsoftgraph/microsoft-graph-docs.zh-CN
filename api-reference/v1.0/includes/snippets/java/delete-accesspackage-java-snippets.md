---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8adfe0e6d824a5d2d52d8293319cda19a349b17d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338030"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{accessPackageId}")
    .buildRequest()
    .delete();

```