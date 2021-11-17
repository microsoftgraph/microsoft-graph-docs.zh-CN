---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a5aebd9b857b9d2e898d91cc00094546c1ebb38f59169864e1df4e4c1065529
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220175"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().windowsHelloForBusinessMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .delete();

```