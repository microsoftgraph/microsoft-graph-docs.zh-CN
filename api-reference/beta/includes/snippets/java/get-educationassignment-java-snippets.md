---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25acdaf39a46fdc31d39b03cf35775495d4e9602
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982886"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = graphClient.education().classes("11014").assignments("19002")
    .buildRequest()
    .get();

```