---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 76c791feb242e11b82fa3fa3206e8051626291ba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867131"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonCollectionPage people = graphClient.me().people()
    .buildRequest()
    .get();

```