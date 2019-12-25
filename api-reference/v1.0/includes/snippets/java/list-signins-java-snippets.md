---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09e3f446180637d300e1996204a69c2d1df1b15f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "35891594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .get();

```