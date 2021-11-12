---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3349492660e9e1fefd4865371a42eaf3208ceafe60be3dfb03838df85b75edfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104082"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.administrativeUnits("{id}")
    .buildRequest()
    .get();

```