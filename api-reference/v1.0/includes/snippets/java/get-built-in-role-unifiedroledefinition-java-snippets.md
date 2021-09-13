---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ad13c6538ef703c8d40fef5a00291a90ee01433
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097848"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinition unifiedRoleDefinition = graphClient.roleManagement().directory().roleDefinitions("fdd7a751-b60b-444a-984c-02652fe8fa1c")
    .buildRequest()
    .get();

```