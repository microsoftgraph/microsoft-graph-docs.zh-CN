---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f345c04a018fd2d1da5b2622a72afc7ce375e0e48e337455c023b47f8951f702
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219994"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .clearFilters()
    .buildRequest()
    .post();

```