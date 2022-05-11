---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61b2ee3433f04f8a55a20d2f51cd6ec7b78bf7c5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327442"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonName()
nickname := "Kesha"
requestBody.SetNickname(&nickname)
personNameId := "personName-id"
graphClient.Me().Profile().NamesById(&personNameId).Patch(requestBody)


```