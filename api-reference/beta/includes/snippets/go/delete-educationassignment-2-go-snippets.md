---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c74f16784cefc57bfe5c8fd557bd3dcb6600033a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412427"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationCategoryId := "educationCategory-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentCategoriesById(&educationCategoryId).Delete(nil)


```