---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51f3bf939c584ba671e82c2b7c335e3a25337f8c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095509"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

workPositionId := "workPosition-id"
result, err := graphClient.Me().Profile().PositionsById(&workPositionId).Get(options)


```