---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f868c01ec66c068531be5d1c136e1cefc4e88c4a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877935"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = True;

graphClient.contacts("{id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```