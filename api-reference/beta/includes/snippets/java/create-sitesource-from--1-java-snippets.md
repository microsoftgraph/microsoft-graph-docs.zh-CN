---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86ce011b464c9d630ff3250f1c182f844c39cc43
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60934642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource siteSource = new SiteSource();
Site site = new Site();
site.webUrl = "https://contoso.sharepoint.com/sites/HumanResources";
siteSource.site = site;

graphClient.compliance().ediscovery().cases("15d80234-8320-4f10-96d0-d98d53ffdfc9").custodians("8904528fef4d4578b44f71a80188f400").siteSources()
    .buildRequest()
    .post(siteSource);

```