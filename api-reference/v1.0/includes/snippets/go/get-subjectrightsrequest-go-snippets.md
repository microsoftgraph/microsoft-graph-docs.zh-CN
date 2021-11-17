---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c567d8926da725ca6347560f4e8af5f12260f49
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024092"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

subjectRightsRequestId := "subjectRightsRequest-id"
result, err := graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Get(options)


```