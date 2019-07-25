---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 918305b79505cebcde3a5374d128d1f25d53a78b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867685"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AutomaticRepliesSetting automaticRepliesSetting = graphClient.customRequest("/me/mailboxSettings/automaticRepliesSetting", AutomaticRepliesSetting.class)
    .buildRequest()
    .get();

```