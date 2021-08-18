---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b087b364a072098fa63b5ae1498636ad2b1a3115ee635338e8728bc2cbecefa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163145"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategory educationCategory = graphClient.education().classes("dacbf757-888d-42ae-b701-5e57cec300ae").assignmentCategories("7f64924d-4cdb-4e54-8c37-c0f3d46f0747")
    .buildRequest()
    .get();

```