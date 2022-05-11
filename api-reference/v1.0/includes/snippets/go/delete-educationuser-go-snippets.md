---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d23335fa2938ea2fc1d526074c2be8f233d4da1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327585"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationUserId := "educationUser-id"
graphClient.Education().UsersById(&educationUserId).Delete()


```