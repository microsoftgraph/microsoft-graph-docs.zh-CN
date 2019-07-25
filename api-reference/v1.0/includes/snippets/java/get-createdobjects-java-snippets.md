---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f241b69ed3d1b5cabe6d2bf92813e097a1b51eb3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888909"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage createdObjects = graphClient.me().createdObjects()
    .buildRequest()
    .get();

```