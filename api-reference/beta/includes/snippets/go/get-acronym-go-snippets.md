---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f762c037471135f3b7282fcc91ac7db4f8ce890e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338850"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

acronymId := "acronym-id"
result, err := graphClient.Search().AcronymsById(&acronymId).Get(nil)


```