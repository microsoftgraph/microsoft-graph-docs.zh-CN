---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cbf1185a86eb003b5c7a464d40acd4dbe09df70b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878216"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = graphClient.groups("f5480dfd-7d77-4d0b-ba2e-3391953cc74a").events("AAMkADVl17IsAAA=").extensions("Com.Contoso.Deal")
    .buildRequest()
    .get();

```