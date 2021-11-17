---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f86d5252e412842bc24b92347bd795c00c44790a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031645"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

tiIndicatorId := "tiIndicator-id"
graphClient.Security().TiIndicatorsById(&tiIndicatorId).Delete(options)


```