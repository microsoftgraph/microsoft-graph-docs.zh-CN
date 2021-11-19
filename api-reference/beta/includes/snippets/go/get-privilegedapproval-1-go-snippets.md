---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35a1cc150a6604c32a6377c43856e84d8ee59860
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedApprovalId := "privilegedApproval-id"
result, err := graphClient.PrivilegedApprovalById(&privilegedApprovalId).Get(options)


```