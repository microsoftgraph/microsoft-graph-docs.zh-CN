---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 619a7f5546d198dbb6800c8b2fd0e8e04d989a15
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032150"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

organizationId := "organization-id"
profileCardPropertyId := "profileCardProperty-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ProfileCardPropertiesById(&profileCardPropertyId).Get(options)


```