---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85adb2a221c346eb9f3ec200b5fff73ebb868e44
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095146"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

softwareOathAuthenticationMethodId := "softwareOathAuthenticationMethod-id"
result, err := graphClient.Me().Authentication().SoftwareOathMethodsById(&softwareOathAuthenticationMethodId).Get(options)


```