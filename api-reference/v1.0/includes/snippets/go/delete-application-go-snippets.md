---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa86895ff21b4e5d7d52841a52118eb205b6a912
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098984"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).Delete(options)


```