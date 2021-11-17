---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e3f4141666a61d76698a7f9df6fb08b4aa055df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).Get(options)


```