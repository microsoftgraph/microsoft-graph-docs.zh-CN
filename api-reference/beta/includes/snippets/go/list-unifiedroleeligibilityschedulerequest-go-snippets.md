---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88244a3c03e7656f16cc543702ab6cb95feaf1b6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031513"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.RoleManagement().Directory().RoleEligibilityScheduleRequests().Get(options)


```