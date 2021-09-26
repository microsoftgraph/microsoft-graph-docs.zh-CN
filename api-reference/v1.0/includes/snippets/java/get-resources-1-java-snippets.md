---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f519ab2a3b07f58e5fe538e518fa85062088873
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767015"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResourceCollectionPage resources = graphClient.education().classes("f4a941ff-9da6-4707-ba5b-0eae93cad0b4").assignments("9018ae7a-9953-4796-a152-4c54e0910922").resources()
    .buildRequest()
    .get();

```