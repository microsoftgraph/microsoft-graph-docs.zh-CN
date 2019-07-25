---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1f5a1bdb5ef1882c4db13520d62f2035245db87a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867135"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage ownedObjects = graphClient.me().ownedObjects()
    .buildRequest()
    .get();

```