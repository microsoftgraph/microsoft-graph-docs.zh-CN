---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8a7f3295d30bbacec2a6ada92ff64f3e39d1ec5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981929"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).Delete(options)


```