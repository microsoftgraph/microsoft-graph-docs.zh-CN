---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40e1dbf4b80d7f327c67c8744840bf2f19e63578
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327158"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentRequests().Get()


```