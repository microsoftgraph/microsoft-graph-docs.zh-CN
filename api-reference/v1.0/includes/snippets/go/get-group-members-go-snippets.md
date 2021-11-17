---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cccb215aa462e60bb2ab855d20907d9a32954cc7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993178"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Members().Get(options)


```