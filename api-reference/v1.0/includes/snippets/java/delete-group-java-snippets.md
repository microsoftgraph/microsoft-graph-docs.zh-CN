---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40109d6e721e16d295a9a7cbb5c6e6ddc8ed501d7126bed38674e0e1cb632789
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278548"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .buildRequest()
    .delete();

```