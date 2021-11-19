---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 701470e2dfc0f23839eacc6fee52c647f0e9e530
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094888"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

workPositionId := "workPosition-id"
graphClient.Me().Profile().PositionsById(&workPositionId).Delete(options)


```