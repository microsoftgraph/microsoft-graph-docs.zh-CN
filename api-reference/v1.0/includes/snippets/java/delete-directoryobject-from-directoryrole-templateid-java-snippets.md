---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8a18dc5c62d7910ce55de11a979db07eb134553
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "53005858"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("roleTemplateId=9f06204d-73c1-4d4c-880a-6edb90606fd8").members("bb165b45-151c-4cf6-9911-cd7188912848").reference()
    .buildRequest()
    .delete();

```