---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc6ca518dc2dc66c217c84e60eaac51d0dd99f74
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010778"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

serviceUpdateMessageId := "serviceUpdateMessage-id"
result, err := graphClient.Admin().ServiceAnnouncement().MessagesById(&serviceUpdateMessageId).Get(options)


```