---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1353fba590320400790716e8248dcc3fc1c6bd2e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977393"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String key = "Base64-encoded-pfx-content";

String password = "password-value";

graphClient.trustFramework().keySets("{id}")
    .uploadPkcs12(key,password)
    .buildRequest()
    .post();

```