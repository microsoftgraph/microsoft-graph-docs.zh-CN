---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0aa604a00348fcc89abf3cd40809bce6e53d7ff
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015145"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
graphClient.GroupsById(&groupId).UnsubscribeByMail().Post(options)


```