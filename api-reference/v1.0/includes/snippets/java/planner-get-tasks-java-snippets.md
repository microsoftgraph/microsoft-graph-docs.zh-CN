---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad60d4af05ea55c9533e631aa7436547c97eed6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980855"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().tasks()
    .buildRequest()
    .get();

```