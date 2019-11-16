---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50be551aee9bb60544cd1215d7b453612d28a252
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637804"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerTaskCollectionPage tasks = graphClient.me().planner().tasks()
    .buildRequest()
    .get();

```