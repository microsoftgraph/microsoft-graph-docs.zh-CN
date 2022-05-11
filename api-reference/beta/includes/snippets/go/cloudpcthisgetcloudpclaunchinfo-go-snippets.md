---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5799c7c17ee4017380a5aaa7215d69aaa23deec
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327139"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPCId := "cloudPC-id"
result, err := graphClient.Me().CloudPCsById(&cloudPCId).GetCloudPcLaunchInfo()(cloudPC-id).Get()


```