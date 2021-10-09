---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e90810866cbaaf22c8e71769383df32fd0d0db847a2947c25356b6e672e6f693
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105226"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "2c891f12-928d-4da2-8d83-7d2434a0d8dc";

graphClient.directoryRoles("0afed502-2456-4fd4-988e-3c21924c28a7").members().references()
    .buildRequest()
    .post(directoryObject);

```