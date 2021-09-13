---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 994ae770e6181a83f69bdf66c6c94b7fffe4f575e78f3db0ba22ae127bfed473
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "bb165b45-151c-4cf6-9911-cd7188912848";

graphClient.directoryRoles("roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b").members().references()
    .buildRequest()
    .post(directoryObject);

```