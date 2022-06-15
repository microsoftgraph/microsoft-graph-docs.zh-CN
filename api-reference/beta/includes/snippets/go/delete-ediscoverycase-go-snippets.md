---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a4e4f6efa4afc6365734cbc3c63caf0fbfd22f1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095994"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).Delete()


```