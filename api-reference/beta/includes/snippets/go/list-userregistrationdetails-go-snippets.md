---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5695c4aecc22d4a271d1c704269f961cc468b7dd
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224728"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().AuthenticationMethods().UserRegistrationDetails().Get(nil)


```