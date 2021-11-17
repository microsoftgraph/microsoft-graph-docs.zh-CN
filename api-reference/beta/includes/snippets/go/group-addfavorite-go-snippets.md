---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bfccde84c942df41efe11dd98f28757e1ef9510
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034389"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
graphClient.GroupsById(&groupId).AddFavorite().Post(options)


```