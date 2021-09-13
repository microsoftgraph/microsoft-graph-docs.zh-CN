---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a2ff20981dd6b12cb3acc3e93fc25f37acf0331995f2a8221685ad55c36e8d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161622"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = new EducationRubric();
educationRubric.displayName = "Example Credit Rubric after display name patch";

graphClient.education().me().rubrics("ceb3863e-6912-4ea9-ac41-3c2bb7b6672d")
    .buildRequest()
    .patch(educationRubric);

```