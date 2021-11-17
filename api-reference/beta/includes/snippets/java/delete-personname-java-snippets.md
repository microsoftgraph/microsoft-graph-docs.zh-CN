---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a250a8b2b3d832406f7fb390c5feef4b8a5090654c42004f4d9cbf65ed9a1a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106104"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().names("{id}")
    .buildRequest()
    .delete();

```