---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76c791feb242e11b82fa3fa3206e8051626291ba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882860"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonCollectionPage people = graphClient.me().people()
    .buildRequest()
    .get();

```