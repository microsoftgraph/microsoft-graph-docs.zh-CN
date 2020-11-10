---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46b8cce8c5838fcbc191b50cd5be5a747136a092
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973616"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITimeOffRequestCollectionPage timeOffRequests = graphClient.teams("{teamId}").schedule().timeOffRequests()
    .buildRequest()
    .get();

```