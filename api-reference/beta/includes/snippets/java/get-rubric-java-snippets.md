---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43bed4fd1cd5875a359e333ce648aef41d1b59d78340d4b11262afa17650c79e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278343"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = graphClient.education().classes("{id}").assignments("{id}").rubric()
    .buildRequest()
    .get();

```