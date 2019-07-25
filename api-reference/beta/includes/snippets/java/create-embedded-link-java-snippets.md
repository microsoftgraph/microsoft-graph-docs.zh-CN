---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8bebde034e9513b58d9e23d16990889aaa7969ce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861333"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "embed";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope,expirationDateTime,password,message,recipientsList)
    .buildRequest()
    .post();

```