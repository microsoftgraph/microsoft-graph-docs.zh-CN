---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3875df0741d66385b308820850362a9204bed36f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955308"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSynchronizationErrorCollectionPage errors = graphClient.education().synchronizationProfiles("{id}").errors()
    .buildRequest()
    .get();

```