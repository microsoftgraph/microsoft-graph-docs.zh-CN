---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25986641b09cc27c2753bdee2f95e9536b47b68e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089956"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).AllowedGroups().Get(options)


```