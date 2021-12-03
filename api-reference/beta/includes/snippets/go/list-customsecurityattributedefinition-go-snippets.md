---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cf41d456b9603eedb2309570b3e1ff07039131f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287826"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Get(nil)


```