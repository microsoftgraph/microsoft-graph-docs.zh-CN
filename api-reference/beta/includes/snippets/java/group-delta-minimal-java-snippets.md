---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d7825466141c281a430f9276735d3c151ca994e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954160"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

IGroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,description,mailNickname")
    .get();

```