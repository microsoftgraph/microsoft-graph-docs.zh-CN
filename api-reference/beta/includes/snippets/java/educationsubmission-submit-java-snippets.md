---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eeb8c508d96534725da260114386dd6a821f746
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365833"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("7192332b-e904-4891-81e2-356242ab1858").submissions("02bb5de1-7205-2a25-fe33-f99cf53de1c4")
    .submit()
    .buildRequest()
    .post();

```