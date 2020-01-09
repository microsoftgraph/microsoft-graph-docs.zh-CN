---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b149cd9b63eacdee90e3ce8056b9300456f5553c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637863"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerTaskCollectionPage tasks = graphClient.planner().buckets("{task-id}").tasks()
    .buildRequest()
    .get();

```