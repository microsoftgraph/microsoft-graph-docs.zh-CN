---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ce5960f21f9f4107b5af9e70fcae4134a002aade9aba1dc691e9119d038da29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221215"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().skills("{id}")
    .buildRequest()
    .delete();

```