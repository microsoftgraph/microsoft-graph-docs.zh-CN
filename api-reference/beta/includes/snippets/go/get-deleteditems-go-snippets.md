---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1bc6a663d2977bf2b9ac0ba62943425162d308c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987048"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

directoryObjectId := "directoryObject-id"
result, err := graphClient.Directory().DeletedItemsById(&directoryObjectId).Get(options)


```