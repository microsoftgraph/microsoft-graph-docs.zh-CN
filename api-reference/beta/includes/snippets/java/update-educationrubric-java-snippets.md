---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5a89abbb717b023fab5a4ec14e0565a75a27b1d1aae92c62010a14ebda78051
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221124"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = new EducationRubric();
educationRubric.displayName = "Example Credit Rubric after display name patch";

graphClient.education().me().rubrics("{id}")
    .buildRequest()
    .patch(educationRubric);

```