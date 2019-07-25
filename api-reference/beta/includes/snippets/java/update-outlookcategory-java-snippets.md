---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c065e25dd4a0c6225e008bdb48ba66950b1367d2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877771"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = new OutlookCategory();
outlookCategory.color = CategoryColor.PRESET15;

graphClient.me().outlook().masterCategories("bac262b7-485d-4739-b436-e31467d64fac")
    .buildRequest()
    .patch(outlookCategory);

```