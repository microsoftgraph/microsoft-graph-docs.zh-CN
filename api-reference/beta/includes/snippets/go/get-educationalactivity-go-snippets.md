---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7135e3f768389516f42a2be797d37400ebd48eca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032556"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationalActivityId := "educationalActivity-id"
result, err := graphClient.Me().Profile().EducationalActivitiesById(&educationalActivityId).Get(options)


```