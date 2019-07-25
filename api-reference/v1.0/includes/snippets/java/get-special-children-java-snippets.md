---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a071b6fb0542b4cd651e72b081bd7a95eef9cf5d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883205"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.me().drive().special("{special-folder-name}").children()
    .buildRequest()
    .get();

```