---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71f9c1fb3c60aa57f43db9ff4594a10aa7d6bb83
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326338"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
extensionPropertyId := "extensionProperty-id"
result, err := graphClient.ApplicationsById(&applicationId).ExtensionPropertiesById(&extensionPropertyId).Get()


```