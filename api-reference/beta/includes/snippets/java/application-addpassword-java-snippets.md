---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47a33fdfbc4473ced91a807ddfc5b5854632a751
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962275"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.displayName = "Password friendly name";

graphClient.applications("{id}")
    .addPassword(passwordCredential)
    .buildRequest()
    .post();

```