---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3b3a82d8bc54d27ff00789b4ce08a99045a8883
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092277"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().Directory().RoleEligibilityScheduleRequests().Get(options)


```