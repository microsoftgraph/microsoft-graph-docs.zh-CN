---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d910ae42b959dd1417d810fbfbd900cb3cf3d30d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018659"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
eventId := "event-id"
graphClient.GroupsById(&groupId).EventsById(&eventId).Delete(options)


```