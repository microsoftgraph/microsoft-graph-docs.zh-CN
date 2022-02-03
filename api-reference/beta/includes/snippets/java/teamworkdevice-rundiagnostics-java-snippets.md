---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdd81a68dc986f8d08c9655cd699fea377768a9e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347880"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teamwork().devices("0f3ce432-e432-0f3c-32e4-3c0f32e43c0f")
    .runDiagnostics()
    .buildRequest()
    .post();

```