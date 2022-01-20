---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1e0d3a867e8a19f3de03a476326169367522049
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089258"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().cloudPC().roleDefinitions("b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff")
    .buildRequest()
    .delete();

```