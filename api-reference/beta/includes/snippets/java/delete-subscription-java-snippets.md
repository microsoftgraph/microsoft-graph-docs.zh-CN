---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e69df5584684bbc0baf3aeb8112a14206d39b87
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869503"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.subscriptions("{id}")
    .buildRequest()
    .delete();

```