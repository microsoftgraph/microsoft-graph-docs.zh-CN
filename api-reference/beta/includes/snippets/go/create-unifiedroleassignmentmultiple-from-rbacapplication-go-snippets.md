---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f04890507b3469ed298c2d9d29b58b4791e7b8e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097657"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().DeviceManagement().RoleAssignments().Post(options)


```