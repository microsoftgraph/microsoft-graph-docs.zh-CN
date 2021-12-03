---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 063aabc5ad8e91e60946299691cfa829f18d4353
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288184"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityUserFlowId := "identityUserFlow-id"
graphClient.Identity().UserFlowsById(&identityUserFlowId).Delete(nil)


```