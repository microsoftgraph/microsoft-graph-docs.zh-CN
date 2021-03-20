---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ddd7bd641e2b58492abbbeb21131f35ef578a7c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976172"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = graphClient.education().me().rubrics("{id}")
    .buildRequest()
    .get();

```