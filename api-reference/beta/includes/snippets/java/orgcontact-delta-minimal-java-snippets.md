---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06d57c976c252b191566c6b7b547b69b465025e2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974296"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

IOrgContactDeltaCollectionPage delta = graphClient.contacts()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,jobTitle,mail")
    .get();

```