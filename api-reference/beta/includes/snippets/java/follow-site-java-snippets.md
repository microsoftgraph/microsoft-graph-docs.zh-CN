---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15728e022f9f6fc34b0feb1f94e14a344ecd0b23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980652"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Site> valueList = new LinkedList<Site>();
Site value = new Site();
value.id = "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740";

valueList.add(value);
Site value1 = new Site();
value1.id = "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851";

valueList.add(value1);
SiteCollectionResponse siteCollectionResponse = new SiteCollectionResponse();
siteCollectionResponse.value = valueList;
SiteCollectionPage siteCollectionPage = new SiteCollectionPage(siteCollectionResponse, null);

graphClient.users("{user-id}").followedSites()
    .add(SiteAddParameterSet
        .newBuilder()
        .withValue(valueList)
        .build())
    .buildRequest()
    .post();

```