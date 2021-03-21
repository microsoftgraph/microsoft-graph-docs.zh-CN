---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aae5fd30a3d317fac3bb16ee34e44eae1805494
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957163"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage groups = graphClient.termStore().groups()
    .buildRequest()
    .get();

```