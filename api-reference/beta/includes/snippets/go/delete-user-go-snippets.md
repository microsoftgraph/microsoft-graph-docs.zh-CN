---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3004b8afd05b7180bf899cb86970b24575c9603
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092376"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
graphClient.UsersById(&userId).Delete(options)


```