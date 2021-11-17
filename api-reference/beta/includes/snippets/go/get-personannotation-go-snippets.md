---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a964e95a29a16fa6ee4ec13508aa4bdbb998506
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026416"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personAnnotationId := "personAnnotation-id"
result, err := graphClient.Me().Profile().NotesById(&personAnnotationId).Get(options)


```