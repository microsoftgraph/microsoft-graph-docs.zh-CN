---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f9fbba598a7c8bfab2ff5b0819bbb9858fb6e10
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091919"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

trustFrameworkPolicyId := "trustFrameworkPolicy-id"
graphClient.TrustFramework().PoliciesById(&trustFrameworkPolicyId).Delete(options)


```