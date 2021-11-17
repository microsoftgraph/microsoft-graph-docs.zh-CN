---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 545147bc5e58546ca4a7bdbaa81bf107bc863d72d1e57f06cdf847aaed1d4e1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158638"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalogCollectionPage accessPackageCatalogs = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs()
    .buildRequest()
    .get();

```