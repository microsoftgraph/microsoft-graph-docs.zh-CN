---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e2e16b517ffbf6bc6b28371adcd05750d4d759b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092054"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().Directory().RoleAssignmentSchedules().Get(options)


```