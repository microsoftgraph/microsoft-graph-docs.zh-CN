---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 470faeb478736e9be6a03e5fd97d3f06fb18faa3
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254479"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = graphClient.education().classes("{id}").assignments("{id}").rubric()
    .buildRequest()
    .get();

```