---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bfa421fdcffb42ec6ba1c6ec56b7100809c5dbdf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879078"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnenoteSectionCollectionPage sections = graphClient.me().onenote().notebooks("{id}").sections()
    .buildRequest()
    .get();

```