---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 660c75e618e97c1eac3cecacf5310cf0a2c2c48a
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869742"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("871dbd5c-3a6a-4392-bfe1-042452793a50").schedule().timeCards("3895809b-a618-4c0d-86a0-d42b25b7d74f")
    .buildRequest()
    .delete();

```