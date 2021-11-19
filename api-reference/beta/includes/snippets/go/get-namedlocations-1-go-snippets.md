---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae3d391122ec6465e162f0af0bff1f9e1b14bc80
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091060"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Identity().ConditionalAccess().NamedLocations().Get(options)


```