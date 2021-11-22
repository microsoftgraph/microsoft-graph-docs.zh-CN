---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a5ce6c38d87965161ede7c793c487cada1f83999549c54e7ed195a95b22bf4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163142"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().events("{id}")
    .dismissReminder()
    .buildRequest()
    .post();

```