---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81f05c8632587b9732a124fe1112c5b8fbde97fb
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().ActivityBasedTimeoutPolicies().Get(nil)


```