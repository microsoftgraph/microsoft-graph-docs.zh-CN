---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32159c51cbd850f52cbc2550eaf061aa4fba1b89
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015714"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTask todoTask = graphClient.me().todo().lists("AAMkADA1MTHgwAAA=").tasks("721a35e2-35e2-721a-e235-1a72e2351a72")
    .buildRequest()
    .get();

```