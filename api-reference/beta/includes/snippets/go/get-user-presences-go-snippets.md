---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f93cd1747a4eff079b73346a257cd83dbac117d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287739"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

presenceId := "presence-id"
result, err := graphClient.Communications().PresencesById(&presenceId).Get(nil)


```