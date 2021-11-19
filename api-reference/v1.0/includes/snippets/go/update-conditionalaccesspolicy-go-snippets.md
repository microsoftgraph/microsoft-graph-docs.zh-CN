---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e592166321eb551eb57d867c0c181f19231783a4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089316"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

conditionalAccessPolicyId := "conditionalAccessPolicy-id"
graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Patch(options)


```