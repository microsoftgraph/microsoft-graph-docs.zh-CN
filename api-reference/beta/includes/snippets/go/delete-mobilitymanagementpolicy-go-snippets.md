---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f003883d427b4c0bd390b8d7b7395dea3a3f25d4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090254"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mobilityManagementPolicyId := "mobilityManagementPolicy-id"
graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).Delete(options)


```