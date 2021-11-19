---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f78dcabbb6325bbc9d43bce56604973bc7ff4987
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094281"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
itemPatentId := "itemPatent-id"
graphClient.UsersById(&userId).Profile().PatentsById(&itemPatentId).Delete(options)


```