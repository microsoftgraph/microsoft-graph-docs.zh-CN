---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab67980607e8e777aa080dabb760582c5c2e1643
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979369"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = graphClient.me().mailFolders("AAMkAGVmMDEzN")
    .buildRequest()
    .get();

```