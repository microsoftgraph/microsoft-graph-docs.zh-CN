---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 431e1c11883df0f5e31b0acc2c733e0d9be94cf5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983062"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}").mentions("{id}")
    .buildRequest()
    .delete();

```