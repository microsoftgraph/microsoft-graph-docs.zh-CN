---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0047476d53f78c7f67cdc01e59c2e1e67d67c87c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978056"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{user-id}";

graphClient.directoryRoles("{role-objectId}").members().references()
    .buildRequest()
    .post(directoryObject);

```