---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b090b7fa4274d96357f2b97b874548d6d0ad5704
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637947"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerTaskCollectionPage tasks = graphClient.planner().tasks()
    .buildRequest()
    .get();

```