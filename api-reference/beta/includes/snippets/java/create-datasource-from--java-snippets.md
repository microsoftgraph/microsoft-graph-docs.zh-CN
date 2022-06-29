---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60871d2ff1faa752bf02e76cbf90132a923bb95a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440213"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource dataSource = new SiteSource();
Site site = new Site();
site.webUrl = "https://contoso.sharepoint.com/sites/SecretSite";
dataSource.site = site;

graphClient.security().cases().ediscoveryCases("{ediscoveryCaseId}").searches("{ediscoverySearchId}").additionalSources()
    .buildRequest()
    .post(dataSource);

```