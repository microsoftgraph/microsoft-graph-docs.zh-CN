---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a500258b04a7f1a4c3fdcc5314126a561dea3d8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090529"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().InvalidateAllRefreshTokens().Post(options)


```