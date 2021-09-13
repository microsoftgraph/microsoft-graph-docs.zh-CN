---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e52f4850cab45f7cf2ecbcc42f9346e56d27c8e0a01f284d2ef9eda9935c6fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333842"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.directory().administrativeUnits("{id}")
    .buildRequest()
    .get();

```