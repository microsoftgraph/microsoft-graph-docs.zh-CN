---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d6bf5d651d0d72da8645e0daa7be782572f4cd9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446699"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource siteSource = new SiteSource();
Site site = new Site();
site.webUrl = "https://m365x809305.sharepoint.com/sites/Retail";
siteSource.site = site;

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").legalHolds("0053a61a3b6c42738f7606791716a22a").siteSources()
    .buildRequest()
    .post(siteSource);

```