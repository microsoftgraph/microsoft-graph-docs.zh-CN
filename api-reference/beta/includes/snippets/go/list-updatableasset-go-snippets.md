---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42178e0cbdbfeb4cdafb3eb4c7bf6e88f1d13545
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084755"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deploymentId := "deployment-id"
result, err := graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Audience().Members().Get(options)


```