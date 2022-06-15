---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 691969dceee3b6432003616d20c25b7bd11b1946
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095465"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).Close(ediscoveryCase-id).Post()


```