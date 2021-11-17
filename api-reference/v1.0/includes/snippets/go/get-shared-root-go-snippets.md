---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e13ce5b1436dc760ef6362b84724afd28923ebf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012893"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

sharedDriveItemId := "sharedDriveItem-id"
result, err := graphClient.SharesById(&sharedDriveItemId).Get(options)


```