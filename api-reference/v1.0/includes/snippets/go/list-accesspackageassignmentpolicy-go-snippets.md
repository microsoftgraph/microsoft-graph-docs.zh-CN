---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01eae457fd0e59c35f24e04c466a31f059f26bda
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209691"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentPolicies().Get(nil)


```