---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac45734aa171e1f692c61ccce3d2980d3ecf0c49
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287718"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().B2cAuthenticationMethodsPolicy().Get(nil)


```