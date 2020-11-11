---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdafdc2bcd0afd0e546d0b294f7230e6716dd30a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983137"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = false;

graphClient.groups("{id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```