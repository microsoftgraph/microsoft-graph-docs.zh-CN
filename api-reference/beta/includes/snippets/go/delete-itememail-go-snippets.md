---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e99d971b64e774bea66a022f5d98bc0c0b1c60f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018604"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

itemEmailId := "itemEmail-id"
graphClient.Me().Profile().EmailsById(&itemEmailId).Delete(options)


```