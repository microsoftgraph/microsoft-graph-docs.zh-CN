---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e83f8cefa20f46720dac8ecae1c57cb6f3c2ff3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137627"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.ServicePrincipals().Delta()().Get(nil)


```