---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c57e5179c583d16e2173ea463d218c3595e0dd73
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877421"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookTaskGroupCollectionPage taskGroups = graphClient.me().outlook().taskGroups()
    .buildRequest()
    .get();

```