---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9be327af3f1a3197c2520862b3ebbac0d8f3c1d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Schedule.TimeOffRequests
    .Request()
    .DeleteAsync();

```