---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b3ba2ff7bd8f1a94e6bd5f26a0c79c1a0184e11
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327814"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).ReprocessLicenseAssignment(user-id).Post()


```