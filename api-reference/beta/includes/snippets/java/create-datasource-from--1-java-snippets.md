---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99d25c7c32004a6bed8feb5a9ac62eb3b68e5919
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60936875"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource dataSource = new SiteSource();
Site site = new Site();
site.webUrl = "https://contoso.sharepoint.com/sites/SecretSite";
dataSource.site = site;

graphClient.compliance().ediscovery().cases("15d80234-8320-4f10-96d0-d98d53ffdfc9").sourceCollections("39b0bafd920e4360995c62e18a5e8a49").additionalSources()
    .buildRequest()
    .post(dataSource);

```