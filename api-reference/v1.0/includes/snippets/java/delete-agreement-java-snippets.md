---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f53ee9152b29d7816cc7217b6e0b8c4699d18524
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528097"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().termsOfUse().agreements("0ec9f6a6-159d-4dd8-a563-1f0b5935e80b")
    .buildRequest()
    .delete();

```