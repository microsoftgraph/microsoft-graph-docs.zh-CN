---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ebed43848f9f6719269a0d63ff6ce5826d893f061a3092a3a811391637857d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103757"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call call = graphClient.communications().calls("2f1a1100-b174-40a0-aba7-0b405e01ed92")
    .buildRequest()
    .get();

```