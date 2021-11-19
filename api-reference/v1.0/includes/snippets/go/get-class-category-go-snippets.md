---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa7e263ffe44575f15cb27b19340aa30b876b9c6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083116"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationCategoryId := "educationCategory-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentCategoriesById(&educationCategoryId).Get(options)


```