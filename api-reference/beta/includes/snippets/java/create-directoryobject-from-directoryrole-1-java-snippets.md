---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f1291e398686be2472a4a1a628b76d99041d077
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946560"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "0f933635-5b77-4cf4-a577-f78a5eb090a2";

graphClient.directoryRoles("0afed502-2456-4fd4-988e-3c21924c28a7").members().references()
    .buildRequest()
    .post(directoryObject);

```