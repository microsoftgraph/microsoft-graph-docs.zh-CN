---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 473d73ed55762d92f90e82beaf2198913ad5e678
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365846"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("dc1af5c4-8211-4e5d-92e6-f006477c2740").resources("7a686854-6d85-4fc0-9729-e36af26f7deb")
    .buildRequest()
    .delete();

```