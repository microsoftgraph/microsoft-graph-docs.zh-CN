---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb7aba37c21d2c3cb6f9d8ba5b385ff8fd30ce5c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346211"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalogCollectionPage catalogs = graphClient.identityGovernance().entitlementManagement().catalogs()
    .buildRequest()
    .get();

```