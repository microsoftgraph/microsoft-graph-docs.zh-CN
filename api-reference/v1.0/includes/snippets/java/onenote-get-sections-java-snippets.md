---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d00b46323d6679e81e6d1fe3bbafd742058574f2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887974"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnenoteSectionCollectionPage sections = graphClient.me().onenote().sections()
    .buildRequest()
    .get();

```