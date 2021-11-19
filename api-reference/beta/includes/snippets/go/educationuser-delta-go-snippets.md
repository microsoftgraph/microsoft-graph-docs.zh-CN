---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a322a01d7758674418324f30fbf85237275cdd9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084078"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).Get(options)


```