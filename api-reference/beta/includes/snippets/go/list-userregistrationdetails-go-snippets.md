---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2d3aff00dbc267e046fcebc80561835ba8e79a0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326480"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().AuthenticationMethods().UserRegistrationDetails().Get()


```