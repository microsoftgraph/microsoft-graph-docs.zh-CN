---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d63d71c56905bcca7ab3d9894e91948a99680088
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348783"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderId := "identityProvider-id"
result, err := graphClient.IdentityProvidersById(&identityProviderId).Get(nil)


```