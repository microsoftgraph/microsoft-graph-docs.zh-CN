---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76edb5ec26d6e121b917ce9f4dacb5c3a2ac456d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905588"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Web"));

IApplicationCollectionPage applications = graphClient.applications()
    .buildRequest( requestOptions )
    .get();

```