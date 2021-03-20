---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b5186d9d4aafd092591ecbc88b6d5f83a95ed13
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967398"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = graphClient.education().me().assignments("{id}").rubric()
    .buildRequest()
    .get();

```