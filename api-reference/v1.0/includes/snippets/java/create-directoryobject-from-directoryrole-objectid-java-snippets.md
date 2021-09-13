---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13a2d28a157f67a7c697e13d0c36abda9245d2d48a76b92aad9bffa5952eb571
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278585"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "15c1a2d5-9101-44b2-83ab-885db8a647ca";

graphClient.directoryRoles("fe8f10bf-c9c2-47eb-95cb-c26cc85f1830").members().references()
    .buildRequest()
    .post(directoryObject);

```