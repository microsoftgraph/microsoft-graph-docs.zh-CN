---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 918305b79505cebcde3a5374d128d1f25d53a78b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970089"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AutomaticRepliesSetting automaticRepliesSetting = graphClient.customRequest("/me/mailboxSettings/automaticRepliesSetting", AutomaticRepliesSetting.class)
    .buildRequest()
    .get();

```