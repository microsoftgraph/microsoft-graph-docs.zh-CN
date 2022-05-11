---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc11b8a4c7033a3acb53bf68fa4eccd454449d5e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326325"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderId := "identityProvider-id"
graphClient.IdentityProvidersById(&identityProviderId).Delete()


```