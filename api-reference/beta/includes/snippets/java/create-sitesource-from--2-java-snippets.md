---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4504926f904630d944065c453b0f5850f8bb53f6
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211170"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource siteSource = new SiteSource();
siteSource.additionalDataManager().put("site@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/sites/50073f3e-cb22-48e5-95a9-51a3da455181"));

graphClient.compliance().ediscovery().cases("c816dd6f-5af8-40c5-a760-331361e05c60").legalHolds("387566cc-38ae-4e85-ab4b-cd2dd34faa07").siteSources()
    .buildRequest()
    .post(siteSource);

```