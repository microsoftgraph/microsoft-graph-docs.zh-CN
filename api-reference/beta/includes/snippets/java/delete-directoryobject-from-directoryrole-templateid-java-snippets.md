---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28e11c0798c1ae7adf9847acbb3c87b573d91c4bd219750c264e24d202730f36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("roleTemplateId=9f06204d-73c1-4d4c-880a-6edb90606fd8").members("bb165b45-151c-4cf6-9911-cd7188912848").reference()
    .buildRequest()
    .delete();

```