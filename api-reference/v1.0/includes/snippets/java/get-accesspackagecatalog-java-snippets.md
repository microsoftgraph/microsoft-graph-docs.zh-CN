---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb6edbb0dd5484ca37b72045f6eabc820183db34
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61335629"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalog accessPackageCatalog = graphClient.identityGovernance().entitlementManagement().catalogs("b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1")
    .buildRequest()
    .get();

```