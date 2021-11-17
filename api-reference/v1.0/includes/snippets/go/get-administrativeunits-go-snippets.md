---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b82ef241f4019eeab9ab99c73ec48c4a2c4529a7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979696"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Directory().AdministrativeUnits().Get(options)


```