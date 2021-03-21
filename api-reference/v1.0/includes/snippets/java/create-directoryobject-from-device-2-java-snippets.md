---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee79341abc2e395f073292e86a4ad5ed4baf3b03
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959894"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.devices("{id}").registeredUsers().references()
    .buildRequest()
    .post(directoryObject);

```