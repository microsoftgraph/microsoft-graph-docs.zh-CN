---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33e6b824cd4fd0c481bf56ce4ccdcef67ec95553
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091485"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().B2cAuthenticationMethodsPolicy().Get(options)


```