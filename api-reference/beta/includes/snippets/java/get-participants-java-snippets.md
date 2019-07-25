---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fc76b9d938a0aa7cc3b1798b269187766dd908be
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864769"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer <TOKEN>"));

IParticipantCollectionPage participants = graphClient.app().calls("57DAB8B1894C409AB240BD8BEAE78896").participants()
    .buildRequest( requestOptions )
    .get();

```