---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b94ca6d3231357fa8203975d33df228df5ba1380
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

webAccountId := "webAccount-id"
graphClient.Me().Profile().WebAccountsById(&webAccountId).Delete(options)


```