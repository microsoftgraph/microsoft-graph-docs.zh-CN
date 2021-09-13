---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 772d0735b6fcc8aeb078877c4f78a9dc528b094814ed5fd75496fed7591cc81c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409605"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnitCollectionPage administrativeUnits = graphClient.directory().administrativeUnits()
    .buildRequest()
    .get();

```