---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5d177a009b01a814b350a85ac1f7476ea4b7af5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096164"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).Get()


```