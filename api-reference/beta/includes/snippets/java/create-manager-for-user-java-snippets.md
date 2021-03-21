---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ac1df870fac001ef782843e55754c1941c25f1d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977676"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.users("{id}").manager().reference()
    .buildRequest()
    .put(directoryObject);

```