---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a96e6904fa44b232134e12653fb39f07f9814085
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365824"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("1b6df208-ea5a-475c-8dd2-b92f693c928a")
    .publish()
    .buildRequest()
    .post();

```