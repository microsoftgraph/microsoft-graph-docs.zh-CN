---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a5aa0e7cb5ab12d6786cbafdd2fe21c0d5670b83
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890106"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserActivityCollectionPage recent = graphClient.me().activities()
    .recent()
    .buildRequest()
    .get();

```