---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93809120cdab17aba1922d7785a0179aa9d97489
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997085"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printerShareId := "printerShare-id"
graphClient.Print().SharesById(&printerShareId).Delete(options)


```