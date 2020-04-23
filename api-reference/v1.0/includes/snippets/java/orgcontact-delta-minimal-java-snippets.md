---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06d57c976c252b191566c6b7b547b69b465025e2
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43770968"
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