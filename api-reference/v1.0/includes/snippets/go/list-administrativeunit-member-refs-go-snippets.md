---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c5b4420772ff105e0bf8c3b70a6beca3ca5a5d2
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040919"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

administrativeUnitId := "administrativeUnit-id"
result, err := graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).Members().$ref().Get()


```