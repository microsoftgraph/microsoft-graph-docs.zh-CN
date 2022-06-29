---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15e6657101360762fbde00f390efa307d024be1a
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694602"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerShareId := "printerShare-id"
groupId := "group-id"
graphClient.Print().SharesById(&printerShareId).AllowedGroupsById(&groupId).$ref().Delete()


```