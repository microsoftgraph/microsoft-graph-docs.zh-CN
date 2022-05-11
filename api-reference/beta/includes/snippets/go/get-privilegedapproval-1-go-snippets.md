---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e53cfa25ea3d464cffa2805e1dc5462aacf9df3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316000"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedApprovalId := "privilegedApproval-id"
result, err := graphClient.PrivilegedApprovalById(&privilegedApprovalId).Get()


```