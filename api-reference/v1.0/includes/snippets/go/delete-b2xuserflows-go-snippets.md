---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f081a95736bd24eaa1897e755d0ffd3cf31d8e8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082736"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).Delete(options)


```