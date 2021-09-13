---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d18c0ad0e2d4e0ae2c35d9dfcbaffbc43607e499556f013aff259371581fdd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105335"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format()
    .autofitColumns()
    .buildRequest()
    .post();

```