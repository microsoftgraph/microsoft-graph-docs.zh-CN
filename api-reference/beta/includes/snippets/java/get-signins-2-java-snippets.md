---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09e3f446180637d300e1996204a69c2d1df1b15f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969065"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .get();

```