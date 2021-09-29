---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68e8eb06ab747b1556cd792804c6fb6208adefc8
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996168"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("7192332b-e904-4891-81e2-356242ab1858").submissions("02bb5de1-7205-2a25-fe33-f99cf53de1c4")
    .reassign()
    .buildRequest()
    .post();

```