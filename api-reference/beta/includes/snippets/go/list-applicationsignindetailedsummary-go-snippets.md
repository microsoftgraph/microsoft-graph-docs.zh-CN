---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30f49feabc40546464e6d34a001b35a17caff7ef
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096104"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().ApplicationSignInDetailedSummary().Get(nil)


```