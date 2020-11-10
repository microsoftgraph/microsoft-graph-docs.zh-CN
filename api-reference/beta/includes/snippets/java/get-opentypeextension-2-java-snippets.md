---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbf1185a86eb003b5c7a464d40acd4dbe09df70b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975663"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = graphClient.groups("f5480dfd-7d77-4d0b-ba2e-3391953cc74a").events("AAMkADVl17IsAAA=").extensions("Com.Contoso.Deal")
    .buildRequest()
    .get();

```