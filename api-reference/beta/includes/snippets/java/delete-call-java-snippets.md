---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 111ee4187113badf6688d7124e9fd1e976369967
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864800"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.app().calls("{id}")
    .buildRequest()
    .delete();

```