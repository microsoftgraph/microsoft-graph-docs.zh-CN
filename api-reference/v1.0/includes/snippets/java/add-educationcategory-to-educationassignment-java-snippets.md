---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 848c1c62a06606410c03ba31e6eb0e94072ce6d1
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211839"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").categories("ec98f158-341d-4fea-9f8c-14a250d489ac").reference()
    .buildRequest()
    .delete();

```