---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc4beaccdae032f1bd8024adcc98d3f638684a0b
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638031"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage memberOf = graphClient.contacts("{id}").memberOf()
    .buildRequest()
    .get();

```