---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ed70d6d8dd62fbf0ad8d808283b7973d085ee9a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904828"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

Int32 int32 = graphClient.groups("{id}").transitiveMembers().$count()
    .buildRequest( requestOptions )
    .get();

```