---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf5f4a317c90aee6edce3cbc86593475ba50a8aa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945387"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationClassCollectionWithReferencesPage classes = graphClient.education().schools("{school-id}").classes()
    .buildRequest()
    .get();

```