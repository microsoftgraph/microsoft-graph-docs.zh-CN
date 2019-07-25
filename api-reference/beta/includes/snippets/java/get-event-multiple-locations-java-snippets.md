---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0392ee58608082a354a456d967d359f3870f08bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859622"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.me().events("AAMkADAGAADDdm4NAAA=")
    .buildRequest()
    .select("subject,body,bodyPreview,organizer,attendees,start,end,location,locations")
    .get();

```