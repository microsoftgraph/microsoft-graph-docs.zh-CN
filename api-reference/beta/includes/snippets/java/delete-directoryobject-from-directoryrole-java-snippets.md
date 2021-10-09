---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f77f8927549b6da1e75830e411b0421bbf74343b5b8023632ab9750d1321b69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220827"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("f8e85ed8-f66f-4058-b170-3efae8b9c6e5").members("bb165b45-151c-4cf6-9911-cd7188912848").reference()
    .buildRequest()
    .delete();

```