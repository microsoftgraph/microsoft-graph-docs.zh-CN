---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35447ff1f36479083d18b6f8db01587fb403d4d3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092277"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryNoncustodialDataSource ediscoveryNoncustodialDataSource = new EdiscoveryNoncustodialDataSource();
SiteSource dataSource = new SiteSource();
Site site = new Site();
site.webUrl = "https://m365x809305.sharepoint.com/sites/Design-topsecret";
dataSource.site = site;
ediscoveryNoncustodialDataSource.dataSource = dataSource;

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").noncustodialDataSources()
    .buildRequest()
    .post(ediscoveryNoncustodialDataSource);

```