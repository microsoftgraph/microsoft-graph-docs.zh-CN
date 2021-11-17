---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf203b8be9f43da0c678d30709dc0d4d1e5e60b4f3bcc2f6d88c653d34c8fcc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163118"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().tasks("AAMkADIyAAAhrb_QAAA=")
    .buildRequest()
    .delete();

```