---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46b8cce8c5838fcbc191b50cd5be5a747136a092
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963546"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITimeOffRequestCollectionPage timeOffRequests = graphClient.teams("{teamId}").schedule().timeOffRequests()
    .buildRequest()
    .get();

```