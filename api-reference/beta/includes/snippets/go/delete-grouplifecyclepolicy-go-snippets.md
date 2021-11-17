---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61424f32e1ec159dd8fc9dd700191938919b2ccc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986465"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupLifecyclePolicyId := "groupLifecyclePolicy-id"
graphClient.GroupLifecyclePoliciesById(&groupLifecyclePolicyId).Delete(options)


```