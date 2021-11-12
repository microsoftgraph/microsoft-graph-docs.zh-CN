---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bcebd5f5c56adba7be6b9c8af1285eba0273dec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60945627"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource siteSource = new SiteSource();
Site site = new Site();
site.webUrl = "https://contoso.sharepoint.com/sites/SecretSite";
siteSource.site = site;

graphClient.compliance().ediscovery().cases("c816dd6f-5af8-40c5-a760-331361e05c60").legalHolds("387566cc-38ae-4e85-ab4b-cd2dd34faa07").siteSources()
    .buildRequest()
    .post(siteSource);

```