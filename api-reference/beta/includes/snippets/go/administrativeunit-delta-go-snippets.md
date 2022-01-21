---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a8800bb17baeb54ff9ba0e8a65617a56c3a8fc1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137715"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.AdministrativeUnits().Delta()().Get(nil)


```