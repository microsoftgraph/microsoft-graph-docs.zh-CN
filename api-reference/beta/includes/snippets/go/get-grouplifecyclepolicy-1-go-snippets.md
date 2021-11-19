---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 681ca0083b48ca6cd2cd9c6c2ea1fc93ed3bee4c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084192"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupLifecyclePolicyId := "groupLifecyclePolicy-id"
result, err := graphClient.GroupLifecyclePoliciesById(&groupLifecyclePolicyId).Get(options)


```