---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f7efac8a1ac2cef7526c4071f8856376b0a56f0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034046"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Onenote().Sections().Get(options)


```