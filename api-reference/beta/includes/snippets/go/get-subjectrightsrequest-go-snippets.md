---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a5dc4e6291289d1efb8d95f22635430004eb74f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086356"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subjectRightsRequestId := "subjectRightsRequest-id"
result, err := graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Get(options)


```