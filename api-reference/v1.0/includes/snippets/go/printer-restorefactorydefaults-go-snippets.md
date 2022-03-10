---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85069f4141246f8dad1552379642e729fe5e499a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412511"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
graphClient.Print().PrintersById(&printerId).RestoreFactoryDefaults(printer-id).Post(nil)


```