---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50cc6f01d2ffc3c6897614be62ac3951e234d3aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968681"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String newPassword = "newPassword-value";

graphClient.users("{id | userPrincipalName}").authentication().passwordMethods("{id}")
    .resetPassword(newPassword,null)
    .buildRequest()
    .post();

```