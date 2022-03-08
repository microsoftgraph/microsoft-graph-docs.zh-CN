---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ed4683b0bea60dc0008e7a4e460f98fdac4f713
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334826"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.IdentityProtection().ServicePrincipalRiskDetections().Get(nil)


```