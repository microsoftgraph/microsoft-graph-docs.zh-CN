---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf24399ede97c83a929b6e210e3e05a535fa139f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60927057"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NoncustodialDataSource noncustodialDataSource = new NoncustodialDataSource();
noncustodialDataSource.applyHoldToSource = false;
SiteSource dataSource = new SiteSource();
Site site = new Site();
site.webUrl = "https://contoso.sharepoint.com/sites/SecretSite";
dataSource.site = site;
noncustodialDataSource.dataSource = dataSource;

graphClient.compliance().ediscovery().cases("15d80234-8320-4f10-96d0-d98d53ffdfc9").noncustodialDataSources()
    .buildRequest()
    .post(noncustodialDataSource);

```