---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d590f69653548f58e3ef1ba4bacb0b75e217bb0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090465"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.PrivilegedRoleAssignmentRequests().Get(options)


```