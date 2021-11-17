---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f25936bffb3129bfb087a1e28df8e92df7ea9ae5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009860"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
graphClient.UsersById(&userId).Delete(options)


```