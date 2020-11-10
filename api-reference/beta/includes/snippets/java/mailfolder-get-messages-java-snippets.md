---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: face77d2015b1d474d0723250bbb6ef262c05e70
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979276"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMessageCollectionPage messages = graphClient.me().mailFolders("AAMkAGVmMDEzM").messages()
    .buildRequest()
    .get();

```