---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 754084a9514e1f7b26bc62c084812f16a989e332
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093650"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage acceptedSenders = graphClient.groups("{id}").acceptedSenders()
    .buildRequest()
    .get();

```