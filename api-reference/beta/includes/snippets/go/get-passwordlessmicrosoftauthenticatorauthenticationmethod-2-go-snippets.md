---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb45f55b90472733ad77e710fe79139415cd9733
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327971"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().PasswordlessMicrosoftAuthenticatorMethods().Get()


```