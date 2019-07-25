---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a5263ebc64309859f70f5aaa07ff3c9d2fb44f0e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881736"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .delete();

```