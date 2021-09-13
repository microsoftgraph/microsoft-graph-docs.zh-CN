---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4a437c1915b57641da8dc6de399ea3dcd311fbdbb1160c02ad1a104becffc74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220968"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").sort()
    .clear()
    .buildRequest()
    .post();

```