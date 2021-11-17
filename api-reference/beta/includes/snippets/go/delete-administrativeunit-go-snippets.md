---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12d579d18e57b3a54e7360b62e2757d00279b29e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991505"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

administrativeUnitId := "administrativeUnit-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).Delete(options)


```