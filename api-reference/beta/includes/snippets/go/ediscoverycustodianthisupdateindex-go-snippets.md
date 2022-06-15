---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3090a9225ea342c73b37174705ffc40657b2c5ed
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095216"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryCustodianId := "ediscoveryCustodian-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).CustodiansById(&ediscoveryCustodianId).UpdateIndex(ediscoveryCase-id, ediscoveryCustodian-id).Post()


```