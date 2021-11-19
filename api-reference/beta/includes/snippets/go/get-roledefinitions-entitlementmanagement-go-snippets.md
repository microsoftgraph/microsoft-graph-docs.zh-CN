---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6675921629080e1bd9e220b6e61efa3ed158488e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103293"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().EntitlementManagement().RoleDefinitions().Get(options)


```