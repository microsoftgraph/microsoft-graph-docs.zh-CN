---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04d2da2c0cd20e37c052426f1e73dfa3811649f4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016238"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationUserId := "educationUser-id"
graphClient.Education().UsersById(&educationUserId).Delete(options)


```