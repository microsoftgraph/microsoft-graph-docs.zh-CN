---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cda27fde4150f9a735289dd9908491c76c9e966
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "53005755"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("f8e85ed8-f66f-4058-b170-3efae8b9c6e5").members("bb165b45-151c-4cf6-9911-cd7188912848").reference()
    .buildRequest()
    .delete();

```