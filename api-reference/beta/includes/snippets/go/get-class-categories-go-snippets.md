---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8d26caf7a156e8d1c3fe5b4aa6af9c0658524ce
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095181"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentCategories().Get(options)


```