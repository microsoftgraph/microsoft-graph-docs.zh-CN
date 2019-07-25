---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 40712faaf001f64d632882730f8e48af98a9f96a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859821"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationClassCollectionPage classes = graphClient.education().me().classes()
    .buildRequest()
    .get();

```