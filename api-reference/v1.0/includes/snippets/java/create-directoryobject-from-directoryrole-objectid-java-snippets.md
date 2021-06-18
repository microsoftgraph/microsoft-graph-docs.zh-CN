---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8209847eb723912d10a8b7a209ea0433277a209
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "53005750"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "15c1a2d5-9101-44b2-83ab-885db8a647ca";

graphClient.directoryRoles("fe8f10bf-c9c2-47eb-95cb-c26cc85f1830").members().references()
    .buildRequest()
    .post(directoryObject);

```