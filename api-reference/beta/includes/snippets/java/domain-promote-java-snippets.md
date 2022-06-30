---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80c1b28d133b86eac16df57ea83cb1fb4d6c7cc4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66446583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("contoso.com")
    .promote()
    .buildRequest()
    .post();

```