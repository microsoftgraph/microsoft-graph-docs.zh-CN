---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dbcddb3fac826408505c5c4319eca59dfd9315c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941695"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationClassCollectionWithReferencesPage classes = graphClient.education().me().classes()
    .buildRequest()
    .get();

```