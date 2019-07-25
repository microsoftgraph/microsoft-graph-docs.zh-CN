---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f6e1b2b4e56154ff75a175f911a1803b74c46197
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879696"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}").mentions("{id}")
    .buildRequest()
    .delete();

```