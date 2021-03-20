---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34cc3003fc80e3402590e9c6754affadf786ee74
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969388"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "alexd@contoso.com";

graphClient.groups("{id}").rejectedSenders().references()
    .buildRequest()
    .post(directoryObject);

```