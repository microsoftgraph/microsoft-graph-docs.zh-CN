---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8555b263d0f702cab5a645dcd650411935f828b1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993304"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).Get(options)


```