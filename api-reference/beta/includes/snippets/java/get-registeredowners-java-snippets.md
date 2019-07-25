---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0f8fde3b224d4d44fff89b28c4a5c260a9472a23
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862719"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage registeredOwners = graphClient.devices("{id}").registeredOwners()
    .buildRequest()
    .get();

```