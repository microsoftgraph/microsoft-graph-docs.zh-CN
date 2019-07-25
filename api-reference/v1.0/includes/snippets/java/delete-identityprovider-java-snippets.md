---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 546828067baea133ed86d95209b88003eaece1cf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889390"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityProviders("Amazon-OAuth")
    .buildRequest()
    .delete();

```