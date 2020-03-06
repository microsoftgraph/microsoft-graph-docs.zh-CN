---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68ee2ad94bbba0e5af477553eff7fc69316ba156
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544199"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "alexd@contoso.com";

graphClient.groups("{id}").rejectedSenders().references()
    .buildRequest()
    .post(directoryObject);

```