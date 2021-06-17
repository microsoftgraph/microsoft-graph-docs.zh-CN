---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d0e86cd331fdfd130b73023cee8d4d458801a22
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990764"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "bb165b45-151c-4cf6-9911-cd7188912848";

graphClient.directoryRoles("roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b").members().references()
    .buildRequest()
    .post(directoryObject);

```