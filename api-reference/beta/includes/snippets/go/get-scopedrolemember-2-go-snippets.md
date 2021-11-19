---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fc4c56e63f1684b35c1a23176175e08b9058807
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089155"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

administrativeUnitId := "administrativeUnit-id"
result, err := graphClient.AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembers().Get(options)


```