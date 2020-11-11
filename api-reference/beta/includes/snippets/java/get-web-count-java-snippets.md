---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 76edb5ec26d6e121b917ce9f4dacb5c3a2ac456d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962073"
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