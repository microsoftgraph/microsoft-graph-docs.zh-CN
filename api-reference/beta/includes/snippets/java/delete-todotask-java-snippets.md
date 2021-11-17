---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7946ce47cd9b81d19891a81634b4191177b5e5a49f07223d8c6032f2d466aaf4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162434"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().todo().lists("AAMkADA1MTHgwAAA=").tasks("721a35e2-35e2-721a-e235-1a72e2351a72")
    .buildRequest()
    .delete();

```