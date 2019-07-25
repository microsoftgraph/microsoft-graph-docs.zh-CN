---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 745a169f23a56664bacbb767bfd48b00d12aaec3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870729"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().schedulingGroups("{schedulingGroupId}")
    .buildRequest()
    .delete();

```