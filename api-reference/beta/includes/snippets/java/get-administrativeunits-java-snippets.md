---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fa71711a82cecc7dae13317280c156dc80450912
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855812"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAdministrativeUnitCollectionPage administrativeUnits = graphClient.administrativeUnits()
    .buildRequest()
    .get();

```