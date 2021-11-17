---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4af3f89db54ba9cccbefb1cbdd09ac2cac447399d019b1eb472adeebc975d68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106649"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .removeFavorite()
    .buildRequest()
    .post();

```