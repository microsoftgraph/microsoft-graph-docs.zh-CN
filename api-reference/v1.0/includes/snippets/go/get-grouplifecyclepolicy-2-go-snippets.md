---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d26630c1f46f449a7dd173b9e461963b635ee97
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61289057"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.GroupLifecyclePolicies().Get(nil)


```