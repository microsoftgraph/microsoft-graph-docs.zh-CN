---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e69e122733e11592d590b428f13ff77ba3b2459
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507363"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategoryCollectionPage categories = graphClient.education().classes("f4a941ff-9da6-4707-ba5b-0eae93cad0b4").assignments("9018ae7a-9953-4796-a152-4c54e0910922").categories()
    .buildRequest()
    .get();

```