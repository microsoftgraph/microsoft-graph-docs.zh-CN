---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6354e50d692cc4424f34bc2f2ccfc278a35705ae
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011639"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
graphClient.Policies().MobileAppManagementPoliciesById(&mobilityManagementPolicyId).Delete(options)


```