---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e57e9a294e8b9c806189c3c043d7393c786fd707
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288072"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personInterestId := "personInterest-id"
graphClient.Me().Profile().InterestsById(&personInterestId).Delete(nil)


```