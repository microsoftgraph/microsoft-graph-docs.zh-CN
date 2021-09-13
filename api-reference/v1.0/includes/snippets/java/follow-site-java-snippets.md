---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec17b195c8f50089a9f5f29d5293d428b2a0132019f6dd872fdba132e34fbeb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378714"
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