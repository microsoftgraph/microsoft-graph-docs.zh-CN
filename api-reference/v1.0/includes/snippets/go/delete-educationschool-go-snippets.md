---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b163df4cef8fd461ca58b5b61bb9dddb0372a0f4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006199"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationSchoolId := "educationSchool-id"
graphClient.Education().SchoolsById(&educationSchoolId).Delete(options)


```