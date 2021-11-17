---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81ff7a2d7646601475037ab6dc8b82f777a482e6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985633"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
personAnnotationId := "personAnnotation-id"
graphClient.UsersById(&userId).Profile().NotesById(&personAnnotationId).Delete(options)


```