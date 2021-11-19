---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01d2a0ec77a015f06759f423ef1c8dacaf68ed21
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101652"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personInterestId := "personInterest-id"
graphClient.Me().Profile().InterestsById(&personInterestId).Delete(options)


```