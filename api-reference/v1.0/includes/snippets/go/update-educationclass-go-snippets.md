---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1388ec24f5a8528892c454c755fe6a41e8e688d2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031058"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).Patch(options)


```