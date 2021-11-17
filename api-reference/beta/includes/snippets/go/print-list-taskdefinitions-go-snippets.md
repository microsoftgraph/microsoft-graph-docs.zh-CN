---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61e6311e79b6f791eafb57ac3e0303f9f127c65e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997344"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Print().TaskDefinitions().Get(options)


```