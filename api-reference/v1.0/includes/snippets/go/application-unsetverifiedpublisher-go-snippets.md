---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a08f2f3a3e015aff254caef7fa9849a76cd672f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996728"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).UnsetVerifiedPublisher().Post(options)


```