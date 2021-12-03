---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de30fa3ba2cfcdd87c06bac4530a10e1a0273d63
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288475"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().CloudPC().RoleAssignments().Get(nil)


```