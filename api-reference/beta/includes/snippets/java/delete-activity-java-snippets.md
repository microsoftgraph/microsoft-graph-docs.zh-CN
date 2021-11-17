---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c98471b02b2b4241a1f8f9ec84706407ae1ed9ff8685f8632e228d8d23fa539
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220607"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().activities("13881113971988980728")
    .buildRequest()
    .delete();

```