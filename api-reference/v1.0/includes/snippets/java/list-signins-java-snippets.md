---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09e3f446180637d300e1996204a69c2d1df1b15f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "35891594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .get();

```