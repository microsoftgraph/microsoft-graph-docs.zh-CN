---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 520b033bb8d290181b90cf36dec14018c74d6fab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025688"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Get(options)


```