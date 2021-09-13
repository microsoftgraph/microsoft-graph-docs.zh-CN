---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b734a3d36b045ac539e695163379491ebea0ab7eaa7465803d0603a07b2cc6c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").sort()
    .reapply()
    .buildRequest()
    .post();

```