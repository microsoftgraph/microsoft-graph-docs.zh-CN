---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 365778eb22dc5f221d3441f5f4604c142aa7b246
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328677"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().HomeRealmDiscoveryPolicies().Get()


```