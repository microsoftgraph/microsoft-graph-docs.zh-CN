---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 605ececf59ada4e125471fe7b34f422e5a7116d2
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905551"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$filter", "hasMembersWithLicenseErrors+eq+true,"));

IGroupCollectionPage groups = graphClient.groups()
    .buildRequest( requestOptions )
    .select("id,displayName")
    .get();

```