---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 045be841e99f1d05d7ce5a0d9fc338f1f584aee9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096011"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSchoolId := "educationSchool-id"
graphClient.Education().SchoolsById(&educationSchoolId).Delete(options)


```