---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1915eb55b64d658c2b0d9ac4b92954beb646f2d7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryObjectId := "directoryObject-id"
result, err := graphClient.Directory().DeletedItemsById(&directoryObjectId).Restore(directoryObject-id).Post()


```