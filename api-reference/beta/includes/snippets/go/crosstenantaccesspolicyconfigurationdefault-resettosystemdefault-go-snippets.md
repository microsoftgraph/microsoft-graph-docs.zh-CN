---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5333e253949c4bc9232824570e2cd0bf48e4d6cd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336443"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

graphClient.Policies().CrossTenantAccessPolicy().Default().ResetToSystemDefault().Post(nil)


```